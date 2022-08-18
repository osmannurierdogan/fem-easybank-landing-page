<template>
  <ul class="links">
    <FooterLinkItem v-for="link in footerLinks" :text="link" :key="link" />
  </ul>
</template>
<style lang="scss" scoped>
@import "@/assets/scss/_shared.scss";
.links {
  display: grid;
  grid-template-columns: 2;
}
</style>

<script>
import FooterLinkItem from "@/components/Footer/FooterLinkItem.vue";
export default {
  name: "FooterLinksComponent",
  components: {
    FooterLinkItem,
  },
  data() {
    return {
      footerLinks: [
        "About Us",
        "Contact",
        "Blog",
        "Careers",
        "Support",
        "Privacy Policy",
      ],
    };
  },
};
</script>
