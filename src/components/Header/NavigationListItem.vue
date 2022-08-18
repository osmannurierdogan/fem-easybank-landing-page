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
  //font-size: 1.4rem;
  font-size: $font-size;
  padding: 1rem auto;
  border: 3px solid transparent;
  border-radius: 0.1rem;
  padding: 2.5rem 1rem;
  transition: all 0.3s;
  cursor: pointer;
  &:hover {
    border-bottom-color: $color-primary-lime-green;
    color: $color-primary-lime-green;
    font-weight: $font-weight-bold;
  }
}
</style>
