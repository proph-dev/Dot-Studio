<template>
    <div class="fixed top-0 left-0 w-full h-full z-10 bg-black/80 flex justify-center items-center">
        <div class="w-[90%] h-[90%] flex rounded-xl overflow-hidden">
            <img :src="require(`~/assets/img/services/${img}`)" :alt="title" class="w-2/3 h-full object-cover" >
            <div class="relative w-1/3 bg-white p-8">
                <CloseModale @click.native="closeModale()" class="hover:scale-110" />
                <h3 class="font-bold text-4xl tracking-wide mb-4 after:content-[''] after:bg-black after:w-1/3 after:h-0.5 after:block after:mt-4">{{ title }}</h3>
                <span class="text-zinc-700 text-sm italic">Projet créé le : <span class="font-semibold">{{ date }}</span></span>
                <p class="font-medium mt-8 leading-8 mb-8">{{ description }}</p>
                <a v-if="this.hasUrl" :href=url target="_blank" rel="noopener noreferrer" class="text-white font-bold uppercase px-8 py-2 rounded bg-cyan-900 hover:bg-cyan-800">Voir le projet</a>                
            </div>
        </div>
    </div>
</template>

<script>
import Paragraph from '../utils/Paragraph.vue';
import CloseModale from './CloseModale.vue';
export default {
  components: { CloseModale, Paragraph },
    props: {
        img: String,
        title: String,
        description: String,
        date: String,
        url: String,
        hasUrl: Boolean
    },
    methods: {
        closeModale() {
            this.$emit('close-ProjectInfos');
        }
    }
}
</script>

<style>

</style>