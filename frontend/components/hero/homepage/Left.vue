<template>
  <div>
    <h1 class="main-title">Your life, <span class="text-cyan-500">Your création</span></h1>
    <Paragraph 
        content="Dot Studio est une entreprise de graphisme qui propose des services professionnels pour
        donner vie à vos projets créatifs, tels que la conception de logo, identité visuelle, brochures, affiches, packaging etc." 
        class="mt-12 text-lg lg:text-xl leading-8" 
    />

    <div class="mt-12 flex flex-col sm:flex-row w-max">
        <CtaButton url="" content="Nous contacter" class="mb-4 sm:mr-4 sm:mb-0" />
        <CtaSecondButton url="" content="En savoir plus"/>
    </div>
  </div>
</template>

<script>
    import Paragraph from '~/components/utils/Paragraph.vue';
    import CtaButton from '~/components/utils/CtaButton.vue';
    import CtaSecondButton from '~/components/utils/CtaSecondButton.vue';

    export default {
        components: {
            Paragraph,
            CtaButton,
            CtaSecondButton
        }
    }
</script>