<template>
  <ul class="navigation__list">
    <NavigationListItem
      v-for="link in navigationLinks"
      :navigationLink="link"
      :key="link"
    />
  </ul>
</template>

<script>
import NavigationListItem from "@/components/Header/NavigationListItem.vue";
export default {
  name: "NavigationList",
  components: {
    NavigationListItem,
  },
  data() {
    return {
      navigationLinks: ["Home", "About", "Contact", "Blog", "Careers"],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/_shared.scss";
.navigation__list {
  display: flex;
  flex-direction: row;
  gap: 2rem;
  font-weight: $font-weight-light;
}
</style>
