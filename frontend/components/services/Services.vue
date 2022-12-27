<template>
    <section class="py-28">
        <div class="container mx-auto">
            <div class="flex flex-col align-center">
                <div class="flex justify-around mx-auto w-full">
                    <Cards v-for="card in cards" v-bind:key="card.id" :img="card.img" :date="card.date" :title="card.title" :intro="card.intro" :url="card.url"/>
                </div>
                <CtaButton url="" content="Voir plus d'articles" class="w-msx mt-12 mx-auto" />
            </div>
        </div>
    </section>
</template>

<script>
export default {

}
</script>