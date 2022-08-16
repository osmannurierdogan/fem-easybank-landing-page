<template>
  <li class="navigation__list__item">
    <a href="#">{{ navigationLink }}</a>
  </li>
</template>

<script>
export default {
  name: "NavigationListItem",
  props: {
    navigationLink: String,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/_shared.scss";
.navigation__list__item {
  color: $color-neutral-grayish-blue;
  font-size: 1.4rem;
}
</style>
