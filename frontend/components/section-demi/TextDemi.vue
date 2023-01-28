<template>
    <section class="py-28">
        <div class="w-[90vw] mx-auto flex flex-col xl:flex-row items-center">
            <div class="w-full xl:w-1/2">
                <h2 class="mb-8 text-center xl:text-left">Rendez votre projet unique <span>grâce à nos designs</span></h2>
                <Paragraph 
                    content="Donnez vie à vos idées avec notre agence de design. Nous créons des designs uniques pour vous aider à mettre en valeur votre projet. Faites confiance à notre expertise pour rendre ce dernier exceptionnel."
                    class="text-[1.2rem] w-full text-center xl:text-left xl:w-3/4"
                />
            </div>

            <div class="w-full xl:w-1/2 flex justify-center relative">
                <!-- Desktop visual -->
                <DesktopAnimation class="hidden md:block" />
                <!-- Mobile visual -->
                <MobileAnimation class="relative md:absolute" />
            </div>
        </div>
    </section>
</template>

<script>
    import Paragraph from '~/components/utils/Paragraph.vue';
    import DesktopAnimation from '~/components/section-demi/DesktopAnimation.vue';
    import MobileAnimation from '~/components/section-demi/MobileAnimation.vue';

    export default {
        components: {
            Paragraph,
            DesktopAnimation,
            MobileAnimation
        }
    }
</script>

<style scoped>
    p {
        @apply text-zinc-500;
    }
</style>