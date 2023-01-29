<template>
    <div>
      <header>
        <ServicesHero class="bg-cyan-900" />
      </header>
  
      <main>
        <Portfolio class="bg-slate-100" />
        <CtaSection />
        <TextSection img="photographie-dot-studio.jpg" alt="Photographie DOT Studio" title="Je n'ai pas d'idées" text="
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Explicabo mollitia soluta ipsa laudantium ipsum, quam, est quidem nobis molestias pariatur in quos, 
          repellat dignissimos placeat maiores repudiandae impedit autem nemo? Lorem ipsum dolor sit amet consectetur adipisicing elit. Explicabo mollitia soluta 
          ipsa laudantium ipsum, quam, est quidem nobis molestias pariatur in quos, repellat dignissimos placeat maiores repudiandae impedit autem nemo?
        " />
      </main>
    </div>
  </template>
  
  <script>
  import ServicesHero from '~/components/hero/others-pages/PortfolioHero.vue';
  import Portfolio from '~/components/portfolio/Portfolio.vue';
  import CtaSection from '~/components/utils/CtaSection.vue';
  import TextSection from '~/components/utils/TextSection.vue';
  
  export default {
    components: {
      ServicesHero,
      Portfolio,
      CtaSection,
      TextSection
    }
  }
  </script>
  
  <style>
  
  </style>