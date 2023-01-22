<template>
    <div>
        <h1>{{ article.title }}</h1>
    </div>
</template>

<script>
import articles from '@/datas/articles.json';

export default {
    async asyncData({ params }) {
        const id = parseInt(params.id);
        const article = articles.find(a => a.id === id)
        return { article }
    }
}
</script>

<style>

</style>