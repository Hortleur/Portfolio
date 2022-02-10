<script setup></script>

<template>
  <div class="arrowLeft flex flex-row justify-center items-center h-full">
    <RouterLink to="/about">
      <img
        src="../assets/arrowLeft.svg"
        alt="Fleche vers la gauche"
        width="50"
        class="object-cover"
      />
    </RouterLink>
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
