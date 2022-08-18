<template>
  <!-- <FooterLinkItem v-for="link in footerLinks" :text="link" :key="link" />
  -->
  <div>
    <FooterLinkItem v-for="link in footerLinks" :text="link" :key="link" />
  </div>
</template>
<style lang="scss" scoped>
@import "@/assets/scss/_shared.scss";
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
