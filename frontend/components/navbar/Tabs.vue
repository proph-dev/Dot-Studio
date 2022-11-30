<template>
    <nuxt-link to="/">{{ content }}</nuxt-link>
</template>

<script>
export default {
    props: {
        content: {
            type: String
        }
    }   
}
</script>

<style scoped>

</style>