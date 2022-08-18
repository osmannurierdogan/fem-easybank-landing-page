<template>
  <a href="#" class="footer__link__text">{{ text }}</a>
</template>
<style lang="scss" scoped>
@import "@/assets/scss/_shared.scss";
.footer__link__text {
  &:link,
  &:visited {
    color: $color-neutral-light-grayish-blue;
    font-weight: $font-weight-light;
    font-size: 1.6rem;
  }
}
</style>

<script>
export default {
  name: "FooterLinkItem",
  props: {
    text: String,
  },
};
</script>
