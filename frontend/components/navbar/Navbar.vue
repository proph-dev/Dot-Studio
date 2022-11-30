<template>
    <nav class="flex justify-between px-10 py-4">
        <img src="../../assets/img/logo-dotstudio.svg" alt="Logo de DOT.Studio" class="w-72">
        <div class="flex w-full">
            <Tabs v-for="tab in tabs" v-bind:key="tab.id" :content="tab.content" class="flex items-center text-2xl text-zinc-500 mx-4 first:ml-8"/>
        </div>
    </nav>
</template>

<script>
    import Tabs from '~/components/navbar/Tabs.vue';

    export default {
        components: {
            Tabs
        },
        data() {
        return {
          tabs: [
            {
              id: 1,
              content: "Accueil"
            },
            {
              id: 2,
              content: "Services"
            },
            {
              id: 3,
              content: "À propos"
            },
            {
              id: 4,
              content: "Nous contacter"
            }
          ]
        }
      }
    }
</script>