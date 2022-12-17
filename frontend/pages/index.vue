<template>
<div>
  <!-- Header -->
  <header>
    <!-- Hero -->
    <Hero class="bg-slate-100" />
  </header>

  <!-- Page content -->
  <main>
    <!-- Pourquoi nous ? -->
    <TextDemi class="color-section" />

    <!-- Articles -->
    <Articles class="bg-cyan-900" />

    <!-- Ils nous font confiance -->
    <Partners class="color-section" />
  </main>

  <!-- Footer -->
  <Footer />
</div>

</template>

<script>
import Hero from '~/components/homepage/hero/Hero.vue';
import TextDemi from '~/components/section-demi/TextDemi.vue';
import Articles from '~/components/blog/Articles.vue';
import Partners from '~/components/partners/Partners.vue';
import Footer from '~/components/footer/Footer.vue';

export default {
  name: 'Homepage',
  components: {
    Hero,
    TextDemi,
    Articles,
    Partners,
    Footer
  }
}
</script>

<style scoped>
  .color-section {
    background-color: #F2F1ED;
  }
</style>