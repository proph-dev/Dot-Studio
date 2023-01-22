<template>
    <div class="h-[500px] rounded-2xl overflow-hidden">
        <img :src="require(`~/assets/img/blog/${img}`)" :alt="title" class="h-[40%] w-full object-cover" >
        <div class="bg-white h-[60%] py-8 px-4">
            <span class="text-cyan-500 text-sm font-bold">{{ date }}</span>
            <h3 class="text-2xl font-bold mt-2">{{ title }}</h3>
            <Paragraph :content="intro" class="text-sm mt-2 mb-8" />
            <nuxt-link :to="`/articles/${id}`" class="py-2 px-8 bg-cyan-500 text-white rounded-2xl hover:bg-cyan-400 duration-300 ease-in-out">Voir cet article</nuxt-link>
        </div>
    </div>
</template>

<script>
    import Paragraph from '~/components/utils/Paragraph.vue';

    export default {
        components: {
            Paragraph
        },
        props: {
            id: Number,
            img: {
                type: String,
                required: true
            },
            date: {
                type: String,
                required: true
            },
            title: {
                type: String,
                required: true
            },
            intro: {
                type: String,
                required: true
            },
            img: {
                type: String,
                required: true
            }
        }
    }
</script>