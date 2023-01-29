<template>
    <section class="flex flex-col items-center justify-center py-16 h-max">
        <MainTitle content="Nos services" />
        <p class="text-white w-2/3 text-center">Bienvenue sur notre page de services, vous pourrez découvrir les différents services que nous proposons pour répondre à vos besoins en matière de design. Nous sommes une agence de design professionnelle qui offre des services complets, allant de la conception de logo, de la charte graphique, en passant par l'identité visuelle, les supports de communication, les packaging, et bien plus encore. Nous sommes fiers de pouvoir soutenir nos clients à chaque étape de leur projet pour les aider à atteindre leurs objectifs. N'hésitez pas à explorer nos services et à nous contacter pour discuter de vos besoins et de la façon dont nous pouvons vous aider.</p>
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