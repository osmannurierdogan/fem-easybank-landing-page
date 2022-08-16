<template>
  <Header />
  <Hero />
</template>

<script>
import Header from "@/components/Header/HeaderComponent.vue";
import Hero from "@/components/Hero/HeroComponent.vue";

export default {
  name: "App",
  components: {
    Header,
    Hero,
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
