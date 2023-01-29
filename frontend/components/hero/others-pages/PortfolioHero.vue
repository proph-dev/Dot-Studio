<template>
    <section class="flex flex-col items-center justify-center py-16 h-max">
        <MainTitle content="Portfolio" />
        <p class="text-white w-2/3 text-center">Bienvenue sur notre portfolio, où vous pourrez découvrir les projets les plus récents et les plus réussis de notre agence de design. Nous sommes fiers de partager notre expérience et notre expertise avec vous et espérons que notre travail vous inspirera pour votre propre projet. Nous avons une variété de projets dans différents domaines, allant de la conception de logo, de la charte graphique à l'identité de visuel. Naviguez à travers nos créations et n'hésitez pas à nous contacter pour discuter de votre projet avec nous.</p>
    </section>
</template>

<script>
import MainTitle from '~/components/utils/MainTitle.vue';
import Pragraph from '~/components/utils/Paragraph.vue';

export default {
    components: {
        MainTitle,
        Pragraph
    }
}
</script>