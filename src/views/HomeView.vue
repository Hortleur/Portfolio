<script setup></script>

<template>
  <main>
    <div class="flex flex-col items-center">
      <img
        src="../assets/IMG_20220206_150212.webp"
        alt="photo de moi"
        class="profile rounded-full w-28 md:w-56"
        loading="lazy"
      />
    </div>
    <div
      class="pres bg-gradient-to-t from-blue-500 via-amber-500 to-red-500 bg-opacity-60 py-10 -mt-24 mb-24 mx-4 px-2 md:-mt-32 lg:-mt-40 lg:w-3/5 lg:mx-auto rounded-3xl"
    >
      <h1 class="text-5xl mt-20 font-bold">Kevin Brun</h1>
      <h2 class="text-4xl my-6 font-semibold">Développeur Web Junior Full Stack</h2>
      <p class="text-lg">
        Après avoir travaillé dans l'animation, puis dans la restauration en passant par
        le milieu hospitalier, à presque 30 ans, je me lance dans cette nouvelle aventure
        qu'est le monde du developpement web, un domaine qui m'a toujours attiré.
      </p>
      <div class="flex flex-row justify-around mt-4 -mb-8">
        <a
          href="https://github.com/Hortleur?tab=repositories"
          target="_blank"
          rel="noopener noreferrer"
          ><img
            src="../assets/github-seeklogo.com.svg"
            alt="Lien GitHub"
            width="60"
            loading="lazy"
        /></a>
        <a
          href="https://www.linkedin.com/in/kevin-brun-dev/"
          target="_blank"
          rel="noopener noreferrer"
        >
          <img
            src="../assets/linkedin-icon-seeklogo.com.svg"
            alt="Lien linkedin"
            width="60"
            loading="lazy"
          />
        </a>
        <a href="mailto:kevin.brun.dev@gmail.com"
          ><img
            src="../assets/gs_email_sign.svg"
            alt="Lien email"
            width="60"
            loading="lazy"
        /></a>
      </div>
    </div>
  </main>
</template>

<style>
.pres {
  animation: slide-top 0.5s cubic-bezier(0.25, 0.46, 0.45, 0.94) both;
}
@keyframes slide-top {
  0% {
    transform: translateY(100%);
  }
  100% {
    transform: translateY(0);
    z-index: 0;
  }
}
.profile {
  animation: slide-down 0.5s ease-in-out both;
}
@keyframes slide-down {
  0% {
    transform: translateY(-100%);
  }
  100% {
    transform: translateY(0%);
    z-index: 20;
    box-shadow: 5px 5px 15px 5px #ffa635;
  }
}
</style>
