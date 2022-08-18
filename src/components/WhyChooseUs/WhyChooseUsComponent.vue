<template>
  <section class="section--grayish-blue">
    <div class="container move-up">
      <div class="product">
        <h2 class="product__title">Why choose Easybank?</h2>
        <p class="product__description">
          We leverage Open Banking to turn your bank account into your financial
          hub. <br />
          Control your finances like never before.
        </p>
        <div class="product__properties">
          <ProductProperty
            v-for="productProperty in productProperties"
            :key="productProperty"
            :product="productProperty"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@import "@/assets/scss/_shared.scss";
.product {
  padding: 6.4rem 0 7.2rem;
  position: inherit;
  z-index: 210;
  /* display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: space-between; */
  &__title {
    color: $color-primary-dark-blue;
    font-size: 3.6rem;
    font-weight: $font-weight-regular;
    line-height: 1.1;
    margin-bottom: 2.8rem;
  }
  &__description {
    color: $color-neutral-grayish-blue;
    font-size: $font-size;
    //width: 50%;
    line-height: 1.5;
    margin-bottom: 6.4rem;
    font-weight: $font-weight-light;
  }
  &__properties {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    gap: 2.8rem;
  }
}
</style>

<script>
import ProductProperty from "@/components/WhyChooseUs/ProductProperty.vue";
export default {
  name: "WhyChooseUsComponent",
  components: {
    ProductProperty,
  },
  data() {
    return {
      productProperties: [
        {
          title: "Online Banking",
          description:
            "Our modern web and mobile applications allow you to keep track of your finances wherever you are in the world.",
          iconName: "online",
          iconText: "Online Banking Icon",
          iconSource: "@/assets/images/icon-online.svg",
        },
        {
          title: "Simple Budgeting",
          description:
            "See exactly where your money goes each month. Receive notifications when you’re close to hitting your limits.",
          iconName: "budgeting",
          iconText: "Simple Budgeting Icon",
          iconSource: "@/assets/images/icon-budgeting.svg",
        },
        {
          title: "Fast Onboarding",
          description:
            "We don’t do branches. Open your account in minutes online and start taking control of your finances right away.",
          iconName: "onboarding",
          iconText: "Fast Onboarding Icon",
          iconSource: "@/assets/images/icon-onboarding.svg",
        },
        {
          title: "Open API",
          description:
            "Manage your savings, investments, pension, and much more from one account. Tracking your money has never been easier.",
          iconName: "api",
          iconText: "Open API Icon",
          iconSource: "@/assets/images/icon-api.svg",
        },
      ],
    };
  },
};
</script>
