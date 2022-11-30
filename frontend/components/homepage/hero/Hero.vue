<template>
    <div class="flex h-full">
        <Left class="w-1/2 flex flex-col justify-center" />
        <Right class="w-1/2 flex items-center" />
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