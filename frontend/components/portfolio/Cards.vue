<template>
    <div>
        <article v-on:click="openProjectInfos = !openProjectInfos" class="relative h-[400px] rounded-2xl overflow-hidden cursor-pointer">
            <img :src="require(`~/assets/img/services/${img}`)" :alt="title" class="w-full h-full object-cover" >
            <div class="overlay absolute bg-gradient-to-t from-black/80 to-black/30 bottom-0 left-0 w-full h-full"></div>
            <h3 class="absolute left-5 bottom-5 font-medium text-2xl tracking-wide text-white">{{ title }}</h3>
            <span class="w-3/4 absolute left-1/2 -translate-x-1/2 top-1/2 -translate-y-1/2 text-center text-white px-8 py-2 border-2 border-white font-semibold hidden rounded">Cliquez pour afficher le projet</span>
        </article>
        <ProjectInfos @close-ProjectInfos="closeProjectInfos" v-if="openProjectInfos" :img="img" :title="title" :description="description" :date="date" :url="url" :hasUrl="hasUrl" />
    </div>
</template>

<script>
import ProjectInfos from './ProjectInfos.vue';

export default {
    components: {
        ProjectInfos
    },
    props: {
        img: String,
        title: String,
        description: String,
        date: String,
        url: String,
        hasUrl: Boolean
    },
    data() {
        return {
            openProjectInfos: false
        }
    },
    methods: {
        closeProjectInfos() {
            this.openProjectInfos = false;
        }
    }
}
</script>

<style scoped>
article:hover .overlay {
    @apply to-black/80;
}

article h3::before {
    content: '';
    position: absolute;
    top: -12px;
    width: 50%;
    height: 2px;
    background-color: #fff;
}

article:hover span {
    display: block;
}
</style>