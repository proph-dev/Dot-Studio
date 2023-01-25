<template>
    <div class="relative py-12 w-[80vw] mx-auto">
        <main v-if="article">
            <div class="flex flex-col items-center mb-16">
                <div class="ariane flex absolute left-0 top-0">
                    <nuxt-link to="/blog" class="relative mr-6 font-semibold hover:underline" >Blog</nuxt-link>
                    <span>{{ article.title }}</span>
                </div>
                <span class="text-zinc-400 mb-2 text-sm text-center">Publie le {{ article.date }} par {{ article.author }}</span>
                <h1 class="text-center text-5xl font-bold mb-4">{{ article.title }}</h1>
                <Paragraph :content=article.intro class="text-center text-xl lg:w-2/3 mb-8" />
                <img :src="require(`~/assets/img/blog/${article.img}`)" :alt="title" class="w-[90%] h-[600px] object-cover" >
            </div>
            <div class="w-[90%] mx-auto">
                <h2 class="text-4xl mb-4">{{ article.firstTitle }}</h2>
                <Paragraph :content=article.firstContent />

                <h2 class="text-4xl mb-4 mt-16">{{ article.secondTitle }}</h2>
                <Paragraph :content=article.secondContent />
            </div>
        </main>

        <div v-else>
            <p class="text-red-500 font-bold">Aucun article n'a été trouvé</p>
        </div>
    </div>
</template>

<script>
import articles from '@/datas/articles.json';
import slugify from 'slugify'
import Paragraph from '../../components/utils/Paragraph.vue';

export default {
  components: { Paragraph },
    async asyncData({ params }) {
        const title = slugify(params.title, {lower: true});
        const article = articles.find(a => slugify(a.title, {lower: true}) === title)
        return { article: article || null }
    },
    data() {
        return {
            article: {}
        }
    },
    computed: {
        title() {
        return this.article ? this.article.title : ''
        },
        intro() {
            return this.article ? this.article.intro : ''
        },
        firstTitle() {
            return this.article ? this.article.firstTitle : ''
        },
        firstContent() {
            return this.article ? this.article.firstContent : ''
        },
        secondTitle() {
            return this.article ? this.article.secondTitle : ''
        },
        secondContent() {
            return this.article ? this.article.secondContent : ''
        }
    }
}
</script>

<style scoped>
.ariane a::after {
    content: '';
    position: absolute;
    right: -13px;
    top: 50%;
    transform: translateY(-50%) rotate(25deg);
    background-color: #000;
    width: 2px;
    height: 15px;
}
</style>