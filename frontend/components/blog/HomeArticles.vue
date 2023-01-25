<template>
    <section class="py-28">
        <div class="w-[90vw] mx-auto">
            <div class=" flex flex-col align-center">
                <h2 class="mb-8 text-center white">Découvrez <span>nos articles</span></h2>
                <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 mx-auto w-full">
                    <Cards v-for="card in cards" v-bind:key="card.id" :img="card.img" :date="card.date" :title="card.title" :intro="card.intro" :url="card.url"/>
                </div>
                <CtaButton url="/blog" content="Voir plus d'articles" class="w-msx mt-12 mx-auto" />
            </div>
        </div>
    </section>
</template>

<script>
    import Cards from '~/components/blog/Cards.vue';
    import CtaButton from '~/components/utils/CtaButton.vue';

    export default {
      components: {
          Cards,
          CtaButton
      },
      data() {
        return {
          cards: [
            {
              id: 1,
              img: "blog-2.jpg",
              date: "22 janvier 2023",
              title: "Titre de l'article 1",
              intro: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.",
              url: "/articles/titre-de-l'article-1"
            },
            {
              id: 2,
              img: "blog-3.webp",
              date: "07 décembre 2022",
              title: "Titre de l'article 2",
              intro: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.",
              url: "/articles/titre-de-l'article-1"
            },
            {
              id: 3,
              img: "blog-4.jpg",
              date: "26 avril 2023",
              title: "Titre de l'article 3",
              intro: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.",
              url: "/articles/titre-de-l'article-1"
            }
          ]
        }
      }
    }
</script>