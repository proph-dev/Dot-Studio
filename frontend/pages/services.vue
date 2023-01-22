<template>
  <div>
    <header>
      <ServicesHero class="bg-cyan-900" />
    </header>

    <main>
      <Services class="bg-slate-100" />
    </main>
  </div>
</template>

<script>
import ServicesHero from '~/components/hero/others-pages/ServicesHero.vue';
import Services from '~/components/services/Services.vue';

export default {
  components: {
    ServicesHero,
    Services
  }
}
</script>

<style>

</style>