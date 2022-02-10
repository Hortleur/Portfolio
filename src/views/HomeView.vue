<script setup></script>

<template>
  <main>
    <div class="flex flex-col items-center">
      <img
        src="../assets/IMG_20220206_150212.webp"
        alt="photo de moi"
        class="rounded-full w-28 md:w-56"
      />
    </div>
    <div
      class="bg-gradient-to-t from-blue-500 via-amber-500 to-red-500 bg-opacity-60 py-10 -mt-24 mb-24 mx-4 px-2 md:-mt-32 lg:-mt-40 lg:w-3/5 lg:mx-auto rounded-3xl"
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
          ><img src="../assets/github-seeklogo.com.svg" alt="Lien GitHub" width="60"
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
          />
        </a>
        <a href="mailto:dev@kevinb.run"
          ><img src="../assets/gs_email_sign.svg" alt="Lien email" width="60"
        /></a>
      </div>
    </div>
  </main>
</template>
