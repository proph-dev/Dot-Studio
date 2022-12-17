<template>
    <section class="flex items-center px-10 lg:pl-10 lg:pr-0 pt-8 lg:pt-0 pb-8 lg:pb-0 h-max lg:h-screen">
        <Left class="w-full lg:w-1/2 flex flex-col justify-center" />
        <Right class="w-full lg:w-1/2 hidden lg:flex items-center justify-center" />
    </section>
</template>

<script>
    import Left from '~/components/homepage/hero/Left.vue';
    import Right from '~/components/homepage/hero/Right.vue';

    export default {
        components: {
            Left,
            Right
        }
    }
</script>