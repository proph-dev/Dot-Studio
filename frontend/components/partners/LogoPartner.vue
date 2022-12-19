<template>
    <a :href="url" target="_blank" rel="noopener noreferrer nofollow" class="logo">
        <img :src="require(`~/assets/img/partners-logo/${img}`)" class="w-[200px]">
    </a>
</template>

<script>
export default {
    props: {
        img: String,
        url: String
    }   
}
</script>

<style scoped>
.logo {
    display: flex;
    justify-content: center;
    align-items: center;
}
</style>