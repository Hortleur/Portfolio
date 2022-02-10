<script setup></script>

<template>
  <div class="flex flex-row justify-center items-center h-full">
    <img src="../assets/arrowDown.svg" alt="Fleche vers le bas" width="50" />
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
