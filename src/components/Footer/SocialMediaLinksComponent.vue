<template>
  <div class="links">
    <SocialMediaLinkItem
      v-for="link in footerLinks"
      :key="link"
      :iconName="link"
    />
  </div>
</template>
<style lang="scss" scoped>
@import "@/assets/scss/_shared.scss";
.links {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
</style>

<script>
import SocialMediaLinkItem from "@/components/Footer/SocialMediaLinkItem.vue";
export default {
  name: "SocialMediaLinksComponent",
  components: {
    SocialMediaLinkItem,
  },
  data() {
    return {
      footerLinks: ["facebook", "youtube", "twitter", "pinterest", "instagram"],
    };
  },
};
</script>
