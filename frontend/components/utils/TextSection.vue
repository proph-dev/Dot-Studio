<template>
  <section class="py-8 lg:py-28">
    <div :class="{'w-[80vw] mx-auto flex flex-col lg:flex-row-reverse': inverse, 'w-[80vw] mx-auto flex flex-col lg:flex-row': !inverse}">
        <div :class="{'lg:w-1/2 flex items-center justify-center lg:justify-end mb-4 lg:mb-0': inverse, 'lg:w-1/2 flex items-center justify-center lg:justify-start mb-4 lg:mb-0' : !inverse}">
            <img :src="require(`~/assets/img/${img}`)" :alt=alt class="sm:w-3/4 rounded-xl object-cover" >
        </div>
        <div class="lg:w-1/2 flex flex-col justify-center text-center lg:text-left">
            <h2 class="mb-4">{{ title }}</h2>
            <Paragraph :content=text class="lg:text-justify" />
        </div>
    </div>
  </section>
</template>

<script>
import Paragraph from './Paragraph.vue';

export default {
    components: { 
        Paragraph 
    },
    props: {
        img: String,
        alt: String,
        title: String,
        text: String,
        inverse: Boolean
    }
}
</script>