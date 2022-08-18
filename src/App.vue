<template>
  <Header />
  <Hero />
  <WhyChooseUs />
  <LatestArticles />
  <Footer />
</template>

<script>
import Header from "@/components/Header/HeaderComponent.vue";
import Hero from "@/components/Hero/HeroComponent.vue";
import WhyChooseUs from "@/components/WhyChooseUs/WhyChooseUsComponent.vue";
import LatestArticles from "@/components/LatestArticles/LatestArticlesComponent.vue";
import Footer from "@/components/Footer/FooterComponent.vue";

export default {
  name: "App",
  components: {
    Header,
    Hero,
    WhyChooseUs,
    LatestArticles,
    Footer,
  },
};
</script>

<style lang="scss">
@import "@/assets/scss/_shared.scss";
/* #app {
  border: 1px solid red;
  margin: 3% 15%;
} */
</style>
