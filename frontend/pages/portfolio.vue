<template>
    <div>
      <header>
        <ServicesHero class="bg-cyan-900" />
      </header>
  
      <main>
        <Portfolio class="bg-slate-100" />
        <CtaSection />
      </main>
    </div>
  </template>
  
  <script>
  import ServicesHero from '~/components/hero/others-pages/PortfolioHero.vue';
  import Portfolio from '~/components/portfolio/Portfolio.vue';
  import CtaSection from '~/components/utils/CtaSection.vue';
  
  export default {
    components: {
      ServicesHero,
      Portfolio,
      CtaSection
    }
  }
  </script>
  
  <style>
  
  </style>