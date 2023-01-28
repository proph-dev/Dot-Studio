<template>
    <div class="h-screen w-full flex justify-center items-center">
        <div class="w-[90vw] sm:w-[80vw] lg:w-[600px] p-8 shadow-2xl bg-white rounded-xl">
            <MainTitle content="Nous contactez" class="text-center mb-2 text-transparent bg-clip-text bg-gradient-to-r from-sky-400 to-cyan-300" />
            <h2 class="text-base font-medium text-center mb-8">Lorem ipsum dolor sit amet consectetur adipisicing elit. Mollitia fuga corrupti dicta obcaecati. Est, magnam excepturi reiciendis.</h2>       
            
            <form class="flex flex-col" :action="formAction" method="POST" >
                <label for="email" class="mb-2">Adresse email <span class="text-red-500">*</span></label>
                <input type="email" name="email" id="email" placeholder="Saisissez votre adresse e-mail" required>

                <div class="flex flex-col sm:flex-row mt-4">
                    <div class="flex flex-col sm:w-1/2 mr-2">
                        <label for="firstName" class="mt-4 mb-2">Prénom <span class="text-red-500">*</span></label>
                        <input type="text" name="firstName" id="firstName" placeholder="Saisissez votre prénom" required>
                    </div>

                    <div class="flex flex-col sm:w-1/2">
                        <label for="lastName" class="mt-4 mb-2">Nom <span class="text-red-500">*</span></label>
                        <input type="text" name="lastName" id="lastName" placeholder="Saisissez votre nom" required>
                    </div>
                </div>

                <label for="subject" class="mt-4 mb-2">Sujet <span class="text-red-500">*</span></label>
                <input type="text" name="subject" id="subject" placeholder="Saisissez votre nom" required>

                <label for="message" class="mt-4 mb-2">Message <span class="text-red-500">*</span></label>
                <textarea name="message" id="message" cols="30" rows="6" placeholder="Votre message" required></textarea>

                <button type="submit" class="text-white font-semibold bg-gradient-to-r from-sky-400 to-cyan-300 px-8 py-2 rounded-xl w-max mx-auto mt-8 hover:from-cyan-300 hover:to-sky-400">Envoyer le message</button>
            </form>
        </div>
    </div>
</template>

<script>
import MainTitle from '../utils/MainTitle.vue';

export default {
    components: {
        MainTitle
    },
    data() {
        return {
            formAction: process.env.FORM_ACTION
        }
    }
}
</script>

<style scoped>
input, textarea {
    @apply outline-none bg-gray-100 rounded-xl px-4 py-2 resize-none;
}
</style>

<style scoped>
h2 {
    line-height: 1.5rem !important;
}
</style>