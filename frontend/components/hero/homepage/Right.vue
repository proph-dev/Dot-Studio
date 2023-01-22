<template>
  <div>
    <lottie :options="lottieOptions" v-on:animCreated="handleAnimation" />
  </div>
</template>

<script>
import animationData from '../../../assets/animations/hero.json';

export default {
  components: {
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
