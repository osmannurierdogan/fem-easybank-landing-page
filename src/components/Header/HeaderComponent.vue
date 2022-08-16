<template>
  <section class="section--white">
    <div class="container">
      <Navigation />
    </div>
  </section>
</template>

<script>
import Navigation from "@/components/Header/NavigationComponent.vue";
export default {
  name: "HeaderComponent",
  components: {
    Navigation,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/_shared.scss";
.container {
  z-index: 10;
}
</style>
