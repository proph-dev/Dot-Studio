<template>
    <section class="py-28">
        <div class="container mx-auto">
            <div class=" flex flex-col align-center">
                <h2 class="mb-8 text-center white">Découvrez <span>nos articles</span></h2>
                <div class="flex justify-around mx-auto w-full">
                    <Cards v-for="card in cards" v-bind:key="card.id" :img="card.img" :date="card.date" :title="card.title" :intro="card.intro" :url="card.url"/>
                </div>
                <CtaButton url="" content="Voir plus d'articles" class="w-msx mt-12 mx-auto" />
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
              img: "blog-1.webp",
              date: "16 décembre 2022",
              title: "Je suis un titre d'article alors c'est bien",
              intro: "Voici l'introduction de cet article, je ne sais pas trop quoi dire ici mais j'aime beaucoup présenter mon article.",
              url: ""
            },
            {
              id: 2,
              img: "blog-1.webp",
              date: "16 décembre 2022",
              title: "Je suis un titre d'article alors c'est bien",
              intro: "Voici l'introduction de cet article, je ne sais pas trop quoi dire ici mais j'aime beaucoup présenter mon article.",
              url: ""
            },
            {
              id: 3,
              img: "blog-1.webp",
              date: "16 décembre 2022",
              title: "Je suis un titre d'article alors c'est bien",
              intro: "Voici l'introduction de cet article, je ne sais pas trop quoi dire ici mais j'aime beaucoup présenter mon article.",
              url: ""
            }
          ]
        }
      }
    }
</script>