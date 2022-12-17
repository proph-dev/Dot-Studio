<template>
    <footer class="bg-cyan-900 py-16">
        <div class="flex container mx-auto">
            <div class="w-1/3 flex justify-center align-center">
                <img src="../../assets/img/logo-dot-studio_white.svg" alt="Logo de DOT.Studio" class="w-[200px]">
            </div>
            <div class="w-2/3 flex justify-around align-center text-white ">
                <ul>
                    <span class="list-title">Navigation</span>
                    <li>
                        <nuxt-link to="">Services</nuxt-link>
                    </li>
                    <li>
                        <nuxt-link to="">Portfolio</nuxt-link>
                    </li>
                    <li>
                        <nuxt-link to="">Nous contacter</nuxt-link>
                    </li>
                </ul>

                <ul>
                    <span class="list-title">Nos services</span>
                    <li>
                        <nuxt-link to="">Graphisme</nuxt-link>
                    </li>
                    <li>
                        <nuxt-link to="">Motion design</nuxt-link>
                    </li>
                    <li>
                        <nuxt-link to="">Photographie</nuxt-link>
                    </li>
                    <li>
                        <nuxt-link to="">Montage photo</nuxt-link>
                    </li>
                </ul>

                <ul>
                    <span class="list-title">Nos projets</span>
                    <li>
                        <a href="http://" target="_blank" rel="noopener noreferrer nofollow">
                            Horyzia
                        </a>
                    </li>
                    <li>
                        <a href="http://" target="_blank" rel="noopener noreferrer nofollow">
                            HCF TEAM
                        </a>
                    </li>
                    <li>
                        <a href="http://" target="_blank" rel="noopener noreferrer nofollow">
                            Jadis Lrmite Pas Nette
                        </a>
                    </li>
                </ul>

                <ul>
                    <span class="list-title">Réseaux sociaux</span>
                    <li>
                        <a href="http://" target="_blank" rel="noopener noreferrer nofollow"></a>
                    </li>
                    <li>
                        <a href="http://" target="_blank" rel="noopener noreferrer nofollow"></a>
                    </li>
                    <li>
                        <a href="http://" target="_blank" rel="noopener noreferrer nofollow"></a>
                    </li>
                </ul>
            </div>
        </div>
        <div>

        </div>
    </footer>
</template>

<style scoped>
.list-title {
    @apply font-semibold text-xl;
}
</style>