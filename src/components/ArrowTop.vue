<script setup></script>

<template>
  <div class="arrowRight flex flex-row justify-center items-center h-full">
    <RouterLink to="/">
      <img src="../assets/arrowTop.svg" alt="Fleche vers le haut" width="50" />
    </RouterLink>
  </div>
</template>

<style scoped>
img {
  animation: slide 1s ease-out infinite alternate both;
}
@keyframes slide {
  0% {
    transform: translateY(0);
  }
  100% {
    transform: translateY(-20px);
  }
}
</style>
