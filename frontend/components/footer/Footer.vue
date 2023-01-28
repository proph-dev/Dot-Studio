<template>
    <footer class="bg-cyan-900 pt-16">
        <div class="flex flex-col lg:flex-row w-[90vw] mx-auto">
            <div class="w-full lg:w-1/4 flex justify-center align-center">
                <img src="../../assets/img/logo-dot-studio_white.svg" alt="Logo de DOT.Studio" class="w-[200px]">
            </div>
            <div class="w-full lg:w-3/4 flex flex-col lg:flex-row justify-around align-center text-white ">
                <nav class="flex flex-col items-center lg:block mt-8">
                    <span class="list-title">Navigation</span>
                    <div class="flex flex-col mt-2 text-center lg:text-left">
                        <nuxt-link to="">Services</nuxt-link>
                        <nuxt-link to="">Portfolio</nuxt-link>
                        <nuxt-link to="">Nous contacter</nuxt-link>
                    </div>
                </nav>

                <nav class="flex flex-col items-center lg:block mt-8">
                    <span class="list-title">Nos services</span>
                    <div class="flex flex-col mt-2 text-center lg:text-left">
                        <nuxt-link to="">Graphisme</nuxt-link>
                        <nuxt-link to="">Motion design</nuxt-link>
                        <nuxt-link to="">Photographie</nuxt-link>
                        <nuxt-link to="">Montage photo</nuxt-link>
                    </div>
                </nav>

                <nav class="flex flex-col items-center lg:block mt-8">
                    <span class="list-title">Nos projets</span>
                    <div class="flex flex-col mt-2 text-center lg:text-left">
                        <a href="http://" target="_blank" rel="noopener noreferrer nofollow">Horyzia</a>
                        <a href="http://" target="_blank" rel="noopener noreferrer nofollow">HCF TEAM</a>
                        <a href="http://" target="_blank" rel="noopener noreferrer nofollow">Jadis Lrmite Pas Nette</a>
                    </div>
                </nav>

                <nav class="flex flex-col items-center lg:block mt-8">
                    <span class="list-title">Réseaux sociaux</span>
                    <div class="flex mt-2">
                        <a href="http://" target="_blank" rel="noopener noreferrer nofollow">
                            <img src="../../assets/img/discord.svg" alt="Icône de Discord" class="w-[48px] mr-4">
                        </a>
                        <a href="http://" target="_blank" rel="noopener noreferrer nofollow">
                            <img src="../../assets/img/instagram.svg" alt="Icône de Discord" class="w-[48px] mr-4">
                        </a>
                        <a href="http://" target="_blank" rel="noopener noreferrer nofollow">
                            <img src="../../assets/img/linkedin.svg" alt="Icône de Discord" class="w-[48px]">
                        </a>
                    </div>
                </nav>
            </div>
        </div>
        <div class="flex justify-center border-t-[1px] border-t-gray-400 mt-16 py-8 text-sm">
            <span class="text-white text-center xs:text-left">© DOT.Studio - Tous Droits Réservés | Site internet par <a href="https://pr0ph.com" target="_blank" rel="noopener noreferrer" class="text-sky-400 hover:underline">Proph</a></span>
        </div>
    </footer>
</template>

<style scoped>
.list-title {
    @apply font-semibold text-xl;
}

nav a {
    @apply mt-1 hover:underline;
}
</style>