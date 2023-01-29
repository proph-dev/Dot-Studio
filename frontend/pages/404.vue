<template>
  <main class="flex flex-col items-center py-16">
    <MainTitle content="Page introuvable" class="text-center text-black" />
    <Paragraph content="La page que vous avez saisi n'existe pas" class="text-center font-semibold text-lg mb-8" />
    <nuxt-link to="/" class="text-center hover:underline">Revenir à l'accueil</nuxt-link>
  </main>
</template>

<script>
import MainTitle from '../components/utils/MainTitle.vue'
import Paragraph from '../components/utils/Paragraph.vue'

export default {
    components: {
        MainTitle,
        Paragraph
    },
    head: {
        title: "Erreur 404 - page introuvable | DOT Studio"
    }

}
</script>