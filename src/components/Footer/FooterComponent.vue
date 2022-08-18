<template>
  <section class="section--dark">
    <div class="container">
      <div class="footer">
        <div class="footer__logo-box">
          <img src="@/assets/images/logo.svg" alt="Easybank Logo" />
          <SocialMediaLinks />
        </div>
        <FooterLinks class="footer__links" />
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
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  justify-content: center;
  align-items: center;
  padding: 4.8rem 0;
  gap: 3.6rem;
  &__logo-box {
    display: flex;
    flex-direction: column;
    gap: 4.8rem;
    & img {
      //filter: brightness(100);
      fill: $color-neutral-white;
      fill-opacity: 1;
    }
  }
  &__links {
    grid-column: 2 / 4;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2.4rem;
    &:nth-child(odd) {
      grid-column: 2 / 3;
    }
    justify-self: center;
  }
  &__copywrite {
    grid-column: 5 / 6;
    display: flex;
    align-items: flex-end;
    justify-content: space-between;
    flex-direction: column;
    color: $color-neutral-grayish-blue;
    //font-size: $font-size;
    font-size: 1.4rem;
    gap: 3.2rem;
  }
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
