<template>
    <article class="relative h-[400px] rounded-2xl overflow-hidden">
        <img :src="require(`~/assets/img/services/${img}`)" :alt="title" class="w-full h-full object-cover" >
        <div class="overlay absolute bg-gradient-to-t from-black/80 to-black/30 bottom-0 left-0 w-full h-full"></div>
        <div class="content absolute left-5 top-[350px] duration-500 ease-in-out">
            <h3 class="font-medium text-2xl tracking-wide text-white">{{ title }}</h3>0
            <p class="text-white leading-7 duration-500 ease-in-out">{{ description }}</p>
        </div>
    </article>
</template>

<script>
    export default {
        props: {
            img: String,
            title: String,
            description: String
        }
    }
</script>

<style scoped>
article:hover .overlay {
    @apply to-black/80;
}

article:hover .content {
    @apply top-10;
}

article h3::before {
    content: '';
    position: absolute;
    top: -12px;
    width: 50%;
    height: 2px;
    background-color: #fff;
}

article:hover h3::before {
    top: 40px;
}
</style>