<template>
    <section class="flex flex-col items-center justify-center py-16 h-max">
        <MainTitle content="Blog" />
        <p class="text-white w-2/3 text-center">Bienvenue sur notre blog, où nous partageons nos connaissances, nos idées sur le monde du design. Nous aborderons des sujets tels que les tendances de l'industrie, les outils de conception et les meilleures pratiques. Nous avons rassemblé ici un contenu riche et varié pour les professionnels et les passionnés de design.</p>
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