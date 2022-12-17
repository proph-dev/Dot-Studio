<template>
    <nav class="flex justify-between items-center px-10 py-4">
      <div class="flex">
        <nuxt-link to="/">
          <img src="../../assets/img/logo-dot-studio.svg" alt="Logo de DOT.Studio" class="w-36">
        </nuxt-link>
        <div class="flex w-full">
            <Tabs v-for="tab in tabs" v-bind:key="tab.id" :content="tab.content" :url="tab.url" class="flex items-center text-xl text-zinc-500 mx-4 first:ml-8"/>
        </div>
      </div>

      <CtaButton url="" content="Nous contacter" class="px-6 py-2" />
    </nav>
</template>

<script>
    import Tabs from '~/components/navbar/Tabs.vue';
    import CtaButton from '~/components/utils/CtaButton.vue';

    export default {
        components: {
            Tabs,
            CtaButton
        },
        data() {
        return {
          tabs: [
            {
              id: 1,
              content: "Accueil",
              url: "/"
            },
            {
              id: 2,
              content: "Services",
              url: "services"
            },
            {
              id: 3,
              content: "Portfolio",
              url: ""
            }
          ]
        }
      }
    }
</script>