<script setup>
import Formulario from './components/Formulario.vue'

</script>

<template>
  <h1 class="titulo">Buscador de Clima</h1>
  <div class="contenedor buscador-clima">
    <Formulario></Formulario> 
  </div> 
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
