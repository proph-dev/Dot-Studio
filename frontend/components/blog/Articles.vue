<template>
    <section class="py-28">
        <div class="container mx-auto">
            <div class=" flex flex-col align-center">
                <h2 class="mb-8 text-center text-cyan-900">Découvrez <span>nos articles</span></h2>
                <div class="grid grid-cols-4 gap-8 mx-auto w-full">
                    <Cards v-for="article in articles" v-bind:key="article.id" :img="article.img" :date="article.date" :title="article.title" :intro="article.intro"/>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
  import Cards from '~/components/blog/Cards.vue';
  import articles from '@/datas/articles.json';

  export default {
    components: {
        Cards
    },
    data() {
      return {
        articles
      }
    }
  }
</script>

<style scoped>
h2 span {
  display: inline;
}
</style>