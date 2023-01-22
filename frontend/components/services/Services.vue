<template>
    <section class="py-28">
        <div class="container mx-auto">
            <div class="flex flex-col align-center">
                <div class="grid grid-cols-2 lg:grid-cols-4 gap-8 mx-auto w-full">
                    <Cards v-for="card in cards" v-bind:key="card.id" :img="card.img" :title="card.title" :description="card.description" />
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
              description: "Notre service de graphisme vous offre des designs uniques et professionnels pour booster votre image de marque. Faites confiance à notre équipe expérimentée pour créer des logos, des brochures, des affiches et plus encore. Faites passer votre message avec style grâce à notre expertise en graphisme."
            },
            {
              id: 2,
              img: "motion-design.webp",
              title: "Motion design",
              description: "Donnez vie à votre projet avec notre service de motion design. Que ce soit pour des vidéos d'animation, des présentations de diapositives animées ou des vidéos publicitaires, notre équipe créative vous proposera des designs uniques et captivants pour une communication efficace. Faites bouger les choses avec notre motion design."
            },
            {
              id: 3,
              img: "photographie.jpg",
              title: "Photographie",
              description: "Captez l'essence de votre entreprise avec notre service de photographie professionnelle. Que ce soit pour des photos de produits, des portraits de l'équipe ou des images de marque, notre équipe expérimentée saura mettre en valeur votre entreprise avec des images de qualité supérieure. Faites une première impression durable avec notre photographie."
            },
            {
              id: 4,
              img: "montage-photo.webp",
              title: "Montage photo",
              description: "Donnez une touche professionnelle à vos photos avec notre service de montage photo. Que ce soit pour des retouches de portrait, la suppression des éléments indésirables ou la création de visuels de marque, notre équipe expérimentée saura transformer vos photos en œuvres d'art visuel. Faites passer votre message avec impact grâce à notre montage photo."
            }
          ]
        }
      }
}
</script>