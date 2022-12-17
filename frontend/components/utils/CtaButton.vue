<template>
    <nuxt-link :to="url" class="text-xl font-medium text-white bg-cyan-500 rounded-xl px-8 py-4 duration-300 ease-in-out hover:bg-cyan-400">{{ content }}</nuxt-link>
</template>

<script>
export default {
    props: {
        content: String,
        url: String
    }
}
</script>