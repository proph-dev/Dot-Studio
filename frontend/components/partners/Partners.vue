<template>
    <section class="py-28">
        <div class="container mx-auto">
            <h2 class="mb-8 text-center">Ils nous ont fait confiance</h2>
            <VueSlickCarousel v-bind="settings">
                <Logo v-for="partner in partners" v-bind:key="partner.id" :img="partner.img" :url="partner.url" />
            </VueSlickCarousel>
        </div>
    </section>
</template>

<script>
  import VueSlickCarousel from 'vue-slick-carousel';
  import 'vue-slick-carousel/dist/vue-slick-carousel.css';
  import Logo from '~/components/partners/LogoPartner.vue';
 
  export default {
    name: 'MyComponent',
    components: { 
        VueSlickCarousel,
        Logo
    },
    data() {
        return {
            settings: {
                "arrows": false,
                "dots": false,
                "infinite": true,
                "slidesToShow": 3,
                "slidesToScroll": 1,
                "autoplay": true,
                "speed": 5000,
                "autoplaySpeed":4000,
            },
            partners: [
            {
              id: 1,
              img: "rap-belge.png",
              url: ""
            },
            {
              id: 2,
              img: "horyzia.png",
              url: "https://horyzia.fr/"
            },
            {
              id: 3,
              img: "logo-dot-studio.svg",
              url: ""
            }
          ]
        }
    }
  }
</script>

<style scoped>
.logo {
    display: flex !important;
    justify-content: center;
    align-content: center;
}
</style>