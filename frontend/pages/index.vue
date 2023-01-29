<template>
<div>
  <!-- Header -->
  <header>
    <!-- Hero -->
    <Hero class="bg-slate-100" />
  </header>

  <!-- Page content -->
  <main>
    <!-- Pourquoi nous ? -->
    <TextDemi class="bg-[#F2F1ED]" />

    <!-- CTA Section -->
    <CtaSection />

    <!-- Articles -->
    <HomeArticles class="bg-cyan-900" />

    <!-- Section texte -->
    <TextSection img="photographie-dot-studio.jpg" alt="Photographie DOT Studio" title="Pourquoi investir dans un graphiste ?" text="
    Lorsqu'il s'agit de promouvoir votre entreprise, il est important de créer une image professionnelle et de se démarquer de la concurrence. 
    C'est là que le travail d'un graphiste professionnel entre en jeu. En investissant dans les services d'un graphiste, vous pourrez bénéficier 
    d'une identité visuelle unique et percutante qui reflète l'essence de votre entreprise. De plus, un graphiste peut également vous aider à élaborer des 
    stratégies de marketing efficaces pour vous faire connaître auprès de votre public cible, en utilisant des designs accrocheurs pour vos supports de communication, 
    vos campagnes publicitaires et vos réseaux sociaux, ce qui peut entraîner une augmentation de vos ventes et de votre notoriété.
    " />

    <TextSection img="photographie-dot-studio.jpg" alt="Photographie DOT Studio" title="Pourquoi nous ?" inverse text="
    Il y a de nombreuses raisons pour lesquelles vous devriez choisir notre agence pour répondre à vos besoins. Tout d'abord, nous avons une 
    équipe expérimentée et qualifiée qui est déterminée à offrir un service de qualité supérieure à chaque client. Nous sommes également très flexibles et 
    réactifs, ce qui signifie que nous pouvons adapter notre approche pour répondre aux besoins spécifiques de chaque client. Nous avons une longue histoire de 
    réussite et de satisfaction des clients, ce qui démontre notre capacité à fournir des résultats exceptionnels à chaque fois. Si vous cherchez une agence 
    fiable et compétente pour répondre à vos besoins, n'hésitez pas à nous contacter. Nous serions ravis de vous aider à réaliser vos projets.
    " />

    <!-- Ils nous font confiance -->
    <Partners class="bg-[#F2F1ED]" />
  </main>
</div>

</template>

<script>
import Hero from '~/components/hero/homepage/Hero.vue';
import TextDemi from '~/components/section-demi/TextDemi.vue';
import HomeArticles from '~/components/blog/HomeArticles.vue';
import Partners from '~/components/partners/Partners.vue';
import CtaSection from '~/components/utils/CtaSection.vue';
import TextSection from '~/components/utils/TextSection.vue';

export default {
  name: 'Homepage',
  components: {
    Hero,
    TextDemi,
    CtaSection,
    HomeArticles,
    TextSection,
    Partners
  }
}
</script>