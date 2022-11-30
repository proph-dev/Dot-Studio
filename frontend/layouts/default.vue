<template>
    <div>
        <Navbar class="lg:fixed top-0 left-0 w-full bg-white"/>
        
        <nuxt/>
    </div>
</template>

<script>
    import Navbar from '~/components/navbar/Navbar.vue';

    export default {
        components: {
            Navbar
        }
    }
</script>

<style>
    /***** General style *****/
    * {
        font-family: 'Poppins';
    }

    /*** H1 ***/
    /* Main Title */
    h1.main-title {
        @apply font-bold text-5xl lg:text-7xl;
    }

    /*** Paragraphs ***/
    p {
        @apply text-zinc-500;
    }

    /*** Buttons ***/
    /* CTA Button */
    .cta-button {
        @apply text-xl font-medium text-white bg-cyan-500 rounded-xl px-8 py-4 duration-300 ease-in-out hover:bg-cyan-400;
    }

    .cta-secondButton {
        @apply text-xl font-medium text-cyan-500 bg-cyan-100 rounded-xl px-8 py-4 duration-300 ease-in-out hover:bg-cyan-200;
    }
</style>