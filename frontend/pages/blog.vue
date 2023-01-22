<template>
    <div>
      <header>
        <BlogHero class="bg-cyan-900" />
      </header>
  
      <main class="articles">
        <Articles class="bg-slate-100" />
      </main>
    </div>
  </template>
  
  <script>
  import BlogHero from '~/components/hero/others-pages/BlogHero.vue';
  import Articles from '~/components/blog/Articles.vue';
  
  export default {
    components: {
        BlogHero,
        Articles
    }
  }
  </script>