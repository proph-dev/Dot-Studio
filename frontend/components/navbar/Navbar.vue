<template>
    <nav class="flex justify-between items-center px-10 py-4">
      <nuxt-link to="/">
        <img src="../../assets/img/logo-dot-studio.svg" alt="Logo de DOT.Studio" class="w-36">
      </nuxt-link>
      <!-- Desktop -->
      <div class="hidden lg:flex justify-between items-center w-full" v-if="!openMenu">
        <div class="flex justify-between">
          <Tabs v-for="tab in tabs" v-bind:key="tab.id" :content="tab.content" :url="tab.url" class="text-xl text-black hover:text-zinc-600 mx-4 first:ml-8"/>
        </div>
        <CtaButton url="/contact" content="Nous contacter" class="px-6 py-[12px] text-lg" />
      </div>

      <!-- Mobile -->
      <div class="absolute top-[87px] left-0 w-full h-[350px] pt-8 bg-white z-10 shadow-2xl rounded-2xl" v-if="openMenu">
        <div class="flex flex-col text-center h-full">
          <Tabs v-for="tab in tabs" v-bind:key="tab.id" :content="tab.content" :url="tab.url" class="text-xl text-black font-medium hover:text-zinc-600 mb-8 last:mb-0"/>
        </div>
        <div class="absolute bottom-8 left-1/2 -translate-x-1/2 w-full sm:w-max flex justify-center">
          <CtaButton url="/contact" content="Nous contacter" />
        </div>
      </div>

      <img src="~/assets/img/icons/hamburger.svg" alt="Menu hamburger" class="lg:hidden h-8 cursor-pointer" v-on:click="openMenu = !openMenu" v-if="!openMenu">
      <img src="~/assets/img/icons/croix.svg" alt="Fermer le menu" class="lg:hidden h-8 cursor-pointer" v-on:click="openMenu = !openMenu" v-if="openMenu">
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
              url: "/services"
            },
            {
              id: 3,
              content: "Portfolio",
              url: "/portfolio"
            },
            {
              id: 4,
              content: "Blog",
              url: "/blog"
            }
          ],
          openMenu: false
        }
      },
      methods: {
        closeMenu() {
            this.openMenu = false;
        }
    }
    }
</script>