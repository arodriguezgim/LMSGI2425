<script setup>
  const nombre = "Alberto";
  const color = "color:red";
  const esMartes = null;
  const dias = ["Lunes", "Martes", "Miercoles"];
  const activo = false;
  //const arrayFrutas = ["🍎", "🍌", "🍉", "🍓", "🍒"];
  const arrayFrutas = [
    {
      name: "Manzana",
      price: "3.00€",
      description: "Manzana Golden",
      stock: 0,
    },
    {
      name: "Limón",
      price: "2.00€",
      description: "limon",
      stock: 5,
    },
    {
      name: "Naranja",
      price: "1.00€",
      description: "Naranja de zumo",
      stock: 2,
    },
  ];

  const objetoFruta = {
    name: "Naranja",
    price: "1.00€",
    description: "Naranja de zumo"
  }

  const hacerClick = ( mensaje ) => {
    console.log( mensaje );
  }
</script>

<template>
  <h1 :style="color">Hola {{ nombre.toLowerCase() }} !!</h1>
  <!--
  <h2> {{ esMartes ? "Hoy es Martes" : "Hoy NO es Martes" }}</h2>
  <h2> {{  dias[2]  }}</h2>
  

  <h2 v-if="esMartes === true">Es MARTES</h2>
  <h2 v-else-if="esMartes === false">NO es martes</h2>
  <h2 v-else>No tengo NI IDEA de Qué día es</h2>

  <h2 v-show="activo">Estoy en true</h2>


  <ul>
    <li v-for="fruta in arrayFrutas" :key="name">
      {{ fruta.name }} - {{  fruta.price }} - {{  fruta.description }}
    </li>

  </ul>

  <h2>Objetos</h2>

  <ul>
    <li v-for="(valor, propiedad, index) in objetoFruta">
      {{ propiedad }} : {{ valor }} : {{ index }}
    </li>
  </ul>
  -->
  <h2>V-if con V-for</h2>
  <template 
      v-for="fruta in arrayFrutas"
      :key="fruta.name">
    <ul>
      <li v-if="fruta.stock > 0"> {{  fruta.name }}</li>
    </ul>
  </template>

  <button @click.left="hacerClick('Click en Boton 1')">Boton Izquierdo</button>
  <button @click.middle="hacerClick('Click en Boton 2')">Boton Centro</button>
  <button @click.right.prevent="hacerClick('Click en Boton 2')">Boton Derecho</button>






</template>

<style>

</style>
 