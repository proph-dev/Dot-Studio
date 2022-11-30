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
    @apply flex items-center pl-10 h-screen;
  }
</style>