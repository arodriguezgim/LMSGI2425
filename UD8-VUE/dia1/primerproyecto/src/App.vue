<script setup>
  const nombre = "Alberto";
  const color = "color:red";
  const esMartes = null;
  const dias = ["Lunes", "Martes", "Miercoles"];
  const activo = false;
  const arrayFrutas = ["🍎", "🍌", "🍉", "🍓", "🍒"];
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
  -->
  <ul>
    <li v-for="(fruta, index) in arrayFrutas" :key="index" >
      {{ index }} - {{ fruta }}
    </li>

  </ul>
</template>

<style>

</style>
 