<template>
    <div class="flex flex-col lg:flex-row h-full">
        <Left class="w-full lg:w-1/2 flex flex-col justify-center" />
        <Right class="w-full lg:w-1/2 hidden lg:flex items-center justify-center" />
    </div>
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