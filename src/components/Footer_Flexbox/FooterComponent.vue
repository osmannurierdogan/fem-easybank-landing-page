<template>
  <section class="section--dark">
    <div class="container">
      <div class="footer">
        <div class="footer__logo-box">
          <img src="@/assets/images/logo.svg" alt="Easybank Logo" />
          <SocialMediaLinks />
        </div>
        <FooterLinks />
        <div class="footer__copywrite">
          <RequestInviteButton />
          <span>&copy; Easybank. All Rights Reserved</span>
        </div>
      </div>
    </div>
  </section>
</template>
<style lang="scss" scoped>
@import "@/assets/scss/_shared.scss";
.footer {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  padding: 6.4rem 0;
  &__logo-box {
    display: flex;
    flex-direction: column;
    gap: 4.8rem;
  }
}
* {
  color: white;
}
</style>

<script>
import RequestInviteButton from "@/components/Shared/RequestInviteButton.vue";
import SocialMediaLinks from "@/components/Footer/SocialMediaLinksComponent.vue";
import FooterLinks from "@/components/Footer/FooterLinksComponent.vue";
export default {
  name: "FooterComponent",
  components: {
    RequestInviteButton,
    SocialMediaLinks,
    FooterLinks,
  },
};
</script>
