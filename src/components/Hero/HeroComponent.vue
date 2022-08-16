<template>
  <section class="section--light-gray">
    <div class="container">
      <!-- <div class="container__fluid"> -->
      <div class="container__hero">
        <div class="container__hero__content">
          <h1 class="container__hero__content__title">
            Next generation digital banking
          </h1>
          <p class="container__hero__content__paragraph">
            Take your financial life online. Your Easybank account will be a
            one-stop-shop for spending, saving, budgeting, investing, and much
            more.
          </p>
          <RequestInviteButton />
        </div>
        <div class="container__hero__image">
          <img
            src="@/assets/images/image-mockups.png"
            alt="easybank image mockups"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import RequestInviteButton from "@/components/Shared/RequestInviteButton";
export default {
  name: "HeroComponent",
  components: {
    RequestInviteButton,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/_shared.scss";
.container {
  &__hero {
    display: flex;
    flex-direction: row;
    background: url(@/assets/images/bg-intro-desktop.svg);
    background-position: bottom bottom;
    background-repeat: no-repeat;
    object-fit: cover;
    gap: 5.4rem;
    &__content {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: center;
      gap: 3.2rem;
      margin: 2rem auto;
      &__title {
        font-weight: $font-weight-light;
        font-size: 5.2rem;
        color: $color-primary-dark-blue;
      }
      &__paragraph {
        color: $color-neutral-grayish-blue;
        font-size: $font-size;
        font-weight: $font-weight-light;
        padding-right: 3rem;
      }
    }
    &__image {
      & img {
        width: 100%;
      }
    }
  }
}
</style>
