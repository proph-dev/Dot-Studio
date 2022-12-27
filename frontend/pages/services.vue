<template>
  <div>
    <header>
      <BannerHero class="bg-cyan-900" />
    </header>

    <main>
      <Services class="bg-slate-100" />
    </main>
  </div>
</template>

<script>
import BannerHero from '~/components/hero/others-pages/BannerHero.vue';
import Services from '~/components/services/Services.vue';

export default {
  components: {
    BannerHero,
    Services
  }
}
</script>

<style>

</style>