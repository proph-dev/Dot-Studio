<template>
    <section class="flex flex-col items-center justify-center py-16 h-max">
        <MainTitle content="Nos services" />
        <p class="text-white w-2/3 text-center">Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorum minus nesciunt eos accusamus similique illo aut id ipsa qui eum voluptatum, enim odit nam adipisci nihil officiis modi neque quam!</p>
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