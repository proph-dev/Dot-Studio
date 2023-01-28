<template>
  <div>
    <header>
      <ServicesHero class="bg-cyan-900" />
    </header>

    <main>
      <Services class="bg-slate-100" />
      <CtaSection />
    </main>
  </div>
</template>

<script>
import ServicesHero from '~/components/hero/others-pages/ServicesHero.vue';
import Services from '~/components/services/Services.vue';
import CtaSection from '~/components/utils/CtaSection.vue';


export default {
  components: {
    ServicesHero,
    Services,
    CtaSection
  }
}
</script>

<style>

</style>