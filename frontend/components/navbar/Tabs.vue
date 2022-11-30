<template>
    <nuxt-link :to="url">{{ content }}</nuxt-link>
</template>

<script>
export default {
    props: {
        content: {
            type: String
        },
        url: {
            type: String
        }
    }   
}
</script>

<style scoped>

</style>