<template>
<div>
  <!-- Header -->
  <header>
    <!-- Hero -->
    <section id="hero">
      <Hero />
    </section>
  </header>

  <!-- Page content -->
  <main class="container mx-auto">

  </main>
</div>

</template>

<script>
import Hero from '~/components/homepage/hero/Hero.vue';

export default {
  name: 'Homepage',
  components: {
    Hero
  }
}
</script>

<style scoped>
  #hero { 
    @apply flex items-center px-10 lg:pl-10 lg:pr-0 pt-8 lg:pt-0 h-max lg:h-screen;
  }
</style>