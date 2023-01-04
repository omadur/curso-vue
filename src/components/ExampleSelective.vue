<template>
  <!--Renderizado selectivo-->
  <h1 v-if="age < 18">Eres menor de edad</h1>
  <h1 v-else>Eres mayor de edad</h1>
  <h1 v-show="age < 18">Esto oculta el elemento html en el DOM</h1>

  // --> Continuar aquí. 25:50
</template>

<script setup>
    let age = 10;
</script>

<style scoped></style>
