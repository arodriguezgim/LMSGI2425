<script setup>
  import { ref, computed } from 'vue';

  const contador = ref(0);

  const sumar = () => {
    contador.value++;

    console.log( contador.value );
  }
</script>

<template>
  <div class="container">
    <h1> Variables reactivas</h1>
    <h2 :class=" contador.value > 5 ? 'verde' : 'rojo'"> {{  contador }}</h2>
    <div class="container">
      <button class="btn btn-primary m-2" @click="sumar()">Incrementar</button>
      <button class="btn btn-warning m-2" @click="sumar()">Resetear</button>
      <button class="btn btn-danger m-2" @click="sumar()">Restar</button>
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

</style>
 