<script setup>
  import { ref, computed } from 'vue';

  const contador = ref(0);

  const arrayFavoritos = ref([]);

  const claseContador = computed( () => {

    if (contador.value === 0) {
      return "zero";
    }
    return contador.value > 0 ? "verde" : "rojo";
  })

  const bloquearBoton = computed( () =>{

    const numero = arrayFavoritos.value.find( (num) => num === contador.value );
    console.log(numero)
    if (contador.value === 0) return true;
    return false;

    //return numero || numero === 0;
  })

  const sumar = () => {
    contador.value++;
  }
  const resetear = () => {
    contador.value = 0;
  }
  const restar = () => {
    contador.value--;
  }
  const anadir = () => {
    arrayFavoritos.value.push( contador.value );
  }
</script>

<template>
  <div class="container">
    <h1> Variables reactivas</h1>
    <h2 :class="claseContador"> {{  contador }}</h2>
    <div class="container">
      <button class="btn btn-primary m-2" @click="sumar()">Incrementar</button>
      <button class="btn btn-warning m-2" @click="resetear()">Resetear</button>
      <button class="btn btn-danger m-2" @click="restar()">Restar</button>
      <button class="btn btn-success m-2" @click="anadir()" :disabled="bloquearBoton">Añadir Favorito</button>
      <br>
      {{ arrayFavoritos }}
    </div>
    
  </div>
  
</template>

<style>

  .rojo {
    color: red;
  }
  .verde {
    color: green;
  }
  .zero {
    color: black;
  }

</style>
 