<script setup></script>

<template>
  <div class="arrowRight flex flex-row justify-center items-center h-full">
    <img src="../assets/arrowRight.svg" alt="Fleche vers la droite" width="50" />
  </div>
</template>

<style scoped>
img {
  animation: slide 1s ease-out infinite alternate both;
}
@keyframes slide {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(-20px);
  }
}
</style>
