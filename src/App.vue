<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <nav class="py-9 text-2xl font-bold text-white flex flex-row justify-center">
    <Router-link to="/" class="mr-2 focus:text-amber-400"> Accueil </Router-link>
    |
    <Router-link to="/PortFolio" class="mx-2 focus:text-amber-400">Portfolio</Router-link>
  </nav>
  <RouterView />
</template>

<style></style>
