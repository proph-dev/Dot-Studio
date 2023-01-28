<template>
    <section class="py-28">
        <div class="flex flex-col lg:flex-row w-[80vw] mx-auto">
            <div class="flex items-center lg:w-1/2">
                <lottie :options="lottieOptions" v-on:animCreated="handleAnimation" />
            </div>
            <div class="flex flex-col justify-center lg:w-1/2">
                <h2 class="mb-4">Avez-vous un projet à créer ?</h2>
                <Paragraph content="Contactez nos experts, ils vous répondront rapidement !" class="text-[1.2rem] mb-8" />
                <CtaButton url="/contact" content="Nous contacter" class="w-max" />
            </div>
        </div>
    </section>
</template>

<script>
import CtaButton from '~/components/utils/CtaButton.vue';
import animationData from '~/assets/animations/cta.json';
import Paragraph from './Paragraph.vue';

export default {
    components: {
        CtaButton,
        Paragraph,
        lottie: require('vue-lottie/src/lottie.vue').default
    },
    data() {
      return {
        anim: {
          animationData: null
        },
        lottieOptions: { animationData }
      };
    },
    methods: {
      handleAnimation: function (anim) {
        this.anim = anim;
      }
    }
}
</script>