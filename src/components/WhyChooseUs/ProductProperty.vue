<template>
  <div :class="`product__property product__property--${product.iconName}`">
    <img
      v-if="product.iconName == 'online'"
      class="product__property__icon"
      src="@/assets/images/icon-online.svg"
      :alt="`${product.iconText}`"
    />
    <img
      v-if="product.iconName == 'budgeting'"
      class="product__property__icon"
      src="@/assets/images/icon-budgeting.svg"
      :alt="`${product.iconText}`"
    />
    <img
      v-if="product.iconName == 'api'"
      class="product__property__icon"
      src="@/assets/images/icon-api.svg"
      :alt="`${product.iconText}`"
    />
    <img
      v-if="product.iconName == 'onboarding'"
      class="product__property__icon"
      src="@/assets/images/icon-onboarding.svg"
      :alt="`${product.iconText}`"
    />
    <!-- <img
      v-if="product.iconName == 'onboarding'"
      class="product__property__icon"
      :src="`@/assets/images/icon-${product.iconName}.svg`"
      :alt="`${product.iconText}`"
    /> -->
    <h3 class="product__property__title">{{ product.title }}</h3>
    <p class="product__property__detail">
      {{ product.description }}
    </p>
  </div>
</template>

<style lang="scss" scoped>
@import "@/assets/scss/_shared.scss";
.product__property {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  flex-direction: column;
  gap: 2.8rem;
  //&__icon {}
  &__title {
    font-weight: $font-weight-regular;
    color: $color-primary-dark-blue;
  }
  &__detail {
    color: $color-neutral-grayish-blue;
    font-size: $font-size;
    //font-size: 1.6rem;
    font-weight: $font-weight-light;
    line-height: 1.4;
    width: 90%;
  }
}
</style>

<script>
export default {
  name: "ProductPropertyComponent",
  components: {},
  props: {
    product: {
      title: String,
      description: String,
      iconName: String,
      iconText: String,
      iconSource: String,
    },
  },
};
</script>
