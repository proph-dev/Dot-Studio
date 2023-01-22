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
    <TextDemi class="bg-[#F2F1ED]" />

    <!-- Articles -->
    <HomeArticles class="bg-cyan-900" />

    <!-- Ils nous font confiance -->
    <Partners class="bg-[#F2F1ED]" />
  </main>
</div>

</template>

<script>
import Hero from '~/components/hero/homepage/Hero.vue';
import TextDemi from '~/components/section-demi/TextDemi.vue';
import HomeArticles from '~/components/blog/HomeArticles.vue';
import Partners from '~/components/partners/Partners.vue';

export default {
  name: 'Homepage',
  components: {
    Hero,
    TextDemi,
    HomeArticles,
    Partners
  }
}
</script>