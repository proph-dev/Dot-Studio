<template>
    <div>
      <header>
        <ServicesHero class="bg-cyan-900" />
      </header>
  
      <main>
        <Portfolio class="bg-slate-100" />
      </main>
    </div>
  </template>
  
  <script>
  import ServicesHero from '~/components/hero/others-pages/PortfolioHero.vue';
  import Portfolio from '~/components/portfolio/Portfolio.vue';
  
  export default {
    components: {
      ServicesHero,
      Portfolio
    }
  }
  </script>
  
  <style>
  
  </style>