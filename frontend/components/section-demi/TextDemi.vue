<template>
    <section class="py-28">
        <div class="container mx-auto flex items-center">
            <div class="w-1/2">
                <h2 class="mb-8">Rendez votre projet unique <span>grâce à nos designs</span></h2>
                <Paragraph 
                    content="Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dolores ea, voluptas nam ratione necessitatibus quas corrupti tempore perspiciatis dolor, voluptate expedita est quisquam fuga cum ipsam blanditiis pariatur doloremque ?"
                    class="text-[1.2rem] w-3/4"
                />
            </div>

            <div class="w-1/2 flex justify-center relative">
                <!-- Desktop visual -->
                <DesktopAnimation />
                <!-- Mobile visual -->
                <MobileAnimation />
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