<template>
    <div>
        <Navbar class="lg:sticky z-10 top-0 left-0 w-full bg-white"/>
        
        <nuxt/>

        <Footer />
    </div>
</template>

<script>
    import Navbar from '~/components/navbar/Navbar.vue';
    import Footer from '~/components/footer/Footer.vue';

    export default {
        components: {
            Navbar,
            Footer
        }
    }
</script>

<style>
    /***** General style *****/
    * {
        font-family: 'Poppins';
    }


    /*** Typo ***/
    /* H1 */
    h1.main-title {
        @apply font-bold text-5xl lg:text-7xl;
    }

    /* H2 */
    h2 {
        @apply font-bold text-3xl lg:text-5xl;
    }

    h2 span {
        @apply block text-cyan-500 mt-2;
    }

    h2.white {
        @apply text-white;
    }

    h2.white span {
        @apply inline text-cyan-300;
    }


    /*** Carousel ***/
    .slick-track {
        display: flex !important;
        align-items: center;
    }
</style>