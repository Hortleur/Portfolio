<script setup></script>
<script>
export default {
  data() {
    return {
      items: [
        {
          id: 0,
          name: "Reservia",
          image:
            "https://xnwpqgpquvsfqmpenpau.supabase.in/storage/v1/object/public/portfolio/projet1.webp",
          altText: "photo du projet Réservia",
          numb: 1,
          objectif: "Intégrer une maquette en utilisant html et css",
          lien: "https://hortleur.github.io/KevinBrun_2_300721/",
        },
        {
          id: 1,
          name: "Ohmyfood",
          image:
            "https://xnwpqgpquvsfqmpenpau.supabase.in/storage/v1/object/public/portfolio/ohmyfood.webp",
          altText: "photo du projet ohmyfood",
          numb: 2,
          objectif: "Dynamiser une page web avec des animations css",
          lien: "https://hortleur.github.io/KevinBrun_3_280821/",
        },
        {
          id: 2,
          name: "La Chouette Agence",
          image:
            "https://xnwpqgpquvsfqmpenpau.supabase.in/storage/v1/object/public/portfolio/chouette1.webp",
          altText: "photo du projet chouette version 1",
          numb: 3,
          objectif:
            "Optimiser un site web existant (SEO & Accéssibilité), ce qui était attendu",
          lien: "https://hortleur.github.io/p4_modifier2/",
        },
        {
          id: 3,
          name: "La Chouette Agence",
          image:
            "https://xnwpqgpquvsfqmpenpau.supabase.in/storage/v1/object/public/portfolio/chouette2.webp",
          altText: "photo du projet chouette version 2",
          numb: "3bis",
          objectif:
            "Optimiser un site web existant (SEO & Accéssibilité), ce que j'aurais fait en situation réelle",
          lien: "https://hortleur.github.io/P4_modifier/",
        },
        {
          id: 4,
          name: "Kanap",
          image:
            "https://xnwpqgpquvsfqmpenpau.supabase.in/storage/v1/object/public/portfolio/kanap.webp",
          altText: "photo du projet Kanap",
          numb: 4,
          objectif: "Faire le front d'un site de e-commerce et le connecter au backend",
          lien: "https://github.com/Hortleur/P5",
        },
        {
          id: 5,
          name: "Hot Takes",
          image:
            "https://xnwpqgpquvsfqmpenpau.supabase.in/storage/v1/object/public/portfolio/gears.webp",
          altText: " illustration pour le projet Hot Takes",
          numb: 5,
          objectif:
            "Construire une Api sécurisée pour un application d'avis gastronomique",
          lien: "https://github.com/Hortleur/backend_P6",
          tech: [
            {
              id: 0,
              name: "MongoDB",
            },
          ],
        },
        {
          id: 6,
          name: "Groupomania",
          image:
            "https://xnwpqgpquvsfqmpenpau.supabase.in/storage/v1/object/public/portfolio/groupomania.webp",
          altText: " photo du projet Groupomania",
          numb: 6,
          objectif: "Créer un réseau social d'entreprise",
          lien: "https://github.com/Hortleur/groupamania",
          tech: [
            {
              id: 0,
              name: "VueJs",
            },
            {
              id: 1,
              name: "Tailwindcss",
            },
            {
              id: 2,
              name: "Prisma",
            },
            {
              id: 3,
              name: "Supabase",
            },
            {
              id: 4,
              name: "Vercel",
            },
          ],
        },
      ],
    };
  },
};
</script>

<template>
  <div>
    <h1 class="text-4xl text-center text-amber-500">Projets OpenClassRooms</h1>
    <div class="lg:flex lg:flex-wrap lg:flex-row lg:justify-evenly">
      <div
        v-for="item in items"
        :key="item.id"
        class="projet my-5 w-4/5 mx-auto border-2 border-emerald-400 rounded-t-xl hover:border-2 hover:border-amber-400 hover:rounded-t-xl lg:w-1/3 lg:mx-2 bg-amber-600"
      >
        <a :href="item.lien" target="_blank" rel="noopener noreferrer">
          <div class="flex flex-row justify-center bg-slate-900 rounded-xl">
            <img
              :src="item.image"
              :alt="item.altText"
              class="rounded-t-lg lg:h-80"
              loading="lazy"
            />
          </div>
          <div class="bg-amber-600 p-2">
            <h2 class="text-3xl">#{{ item.numb }} {{ item.name }}</h2>
            <p>{{ item.objectif }}</p>
            <div class="flex flex-row flex-wrap justify-around bg-slate-100 rounded-2xl">
              <div v-for="item in item.tech" :key="item.id" class="my-2 w-1/3">
                <div class="text-center text-lg text-emerald-900 font-semibolds">
                  <h3 class="font-semibold lg:text-2xl">{{ item.name }}</h3>
                </div>
              </div>
            </div>
          </div>
        </a>
      </div>
    </div>

    <div>
      <h2 class="text-center text-4xl text-amber-500">Projets à venir</h2>
      <h3 class="text-center text-3xl text-amber-500">En construction</h3>
      <div class="flex justify-center mt-4 mb-10">
        <img src="../assets/construction.gif" alt="En construction" />
      </div>
    </div>
  </div>
</template>

<style>
.projet:hover {
  box-shadow: 5px 5px 15px 5px #ffa635;
}
</style>
