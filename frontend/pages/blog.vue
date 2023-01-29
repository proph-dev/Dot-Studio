<template>
    <div>
      <header>
        <BlogHero class="bg-cyan-900" />
      </header>
  
      <main class="articles">
        <Articles class="bg-slate-100" />
        <TextSection img="photographie-dot-studio.jpg" alt="Photographie DOT Studio" title="Je n'ai pas d'idées" text="
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Explicabo mollitia soluta ipsa laudantium ipsum, quam, est quidem nobis molestias pariatur in quos, 
          repellat dignissimos placeat maiores repudiandae impedit autem nemo? Lorem ipsum dolor sit amet consectetur adipisicing elit. Explicabo mollitia soluta 
          ipsa laudantium ipsum, quam, est quidem nobis molestias pariatur in quos, repellat dignissimos placeat maiores repudiandae impedit autem nemo?
        " />
      </main>
    </div>
  </template>
  
  <script>
  import BlogHero from '~/components/hero/others-pages/BlogHero.vue';
  import Articles from '~/components/blog/Articles.vue';
  import TextSection from '~/components/utils/TextSection.vue';
  
  export default {
    components: {
        BlogHero,
        Articles,
        TextSection
    }
  }
  </script>