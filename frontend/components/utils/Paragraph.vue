<template>
    <p>{{ content }}</p>
</template>

<script>
export default {
    props: {
        content: String
    }
}
</script>

<style scoped>
p {
    @apply text-zinc-600;
}
</style>