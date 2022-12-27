<template>
  <div>
    <h1 class="main-title">Your life, <span class="text-cyan-500">Your création</span></h1>
    <Paragraph 
        content="Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dolores ea, voluptas nam ratione necessitatibus quas corrupti tempore perspiciatis dolor, 
        voluptate expedita est quisquam fuga cum ipsam blanditiis pariatur doloremque ?" 
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