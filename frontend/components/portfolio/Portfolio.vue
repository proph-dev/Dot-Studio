<template>
    <section class="py-28">
        <div class="w-[90vw] mx-auto">
            <div class="flex flex-col align-center">
                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8 mx-auto w-full">
                    <Cards v-for="card in cards" v-bind:key="card.id" :img="card.img" :date="card.date" :title="card.title" :description="card.description" :url="card.url" :hasUrl="card.hasUrl" />
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import Cards from "./Cards.vue";

export default {
    components: {
        Cards
    },
    data() {
        return {
          cards: [
            {
              id: 1,
              img: "graphisme.jpg",
              title: "Graphisme",
              description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
              date: "22 janvier 2023",
              hasUrl: true,
              url: "https://google.com/"
            },
            {
              id: 2,
              img: "motion-design.webp",
              title: "Motion Design",
              description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
              date: "05 décembre 2022",
              hasUrl: false,
              url: ""
            },
            {
              id: 3,
              img: "montage-photo.webp",
              title: "Montage photo",
              description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
              date: "15 avril 2023",
              hasUrl: true,
              url: "https://google.com/"
            },
            {
              id: 4,
              img: "photographie.jpg",
              title: "Photographie",
              description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
              date: "13 septembre 2022",
              hasUrl: true,
              url: "https://google.com/"
            }
          ]
        }
      }
}
</script>