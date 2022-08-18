<template>
  <a
    v-if="iconName == 'facebook'"
    :href="`https://www.${iconName}.com`"
    class="footer__social-link"
  >
    <img src="@/assets/images/icon-facebook.svg" :alt="`${iconName} Icon`" />
  </a>
  <a
    v-if="iconName == 'instagram'"
    :href="`https://www.${iconName}.com`"
    class="footer__social-link"
  >
    <img src="@/assets/images/icon-instagram.svg" :alt="`${iconName} Icon`" />
  </a>
  <a
    v-if="iconName == 'pinterest'"
    :href="`https://www.${iconName}.com`"
    class="footer__social-link"
  >
    <img src="@/assets/images/icon-pinterest.svg" :alt="`${iconName} Icon`" />
  </a>
  <a
    v-if="iconName == 'twitter'"
    :href="`https://www.${iconName}.com`"
    class="footer__social-link"
  >
    <img src="@/assets/images/icon-twitter.svg" :alt="`${iconName} Icon`" />
  </a>
  <a
    v-if="iconName == 'youtube'"
    :href="`https://www.${iconName}.com`"
    class="footer__social-link"
  >
    <img src="@/assets/images/icon-youtube.svg" :alt="`${iconName} Icon`" />
  </a>
</template>
<style lang="scss" scoped>
@import "@/assets/scss/_shared.scss";
* {
  color: white;
}
</style>

<script>
export default {
  name: "SocialMediaLinkItem",
  data() {
    return {};
  },
  props: {
    iconName: String,
  },
};
</script>
