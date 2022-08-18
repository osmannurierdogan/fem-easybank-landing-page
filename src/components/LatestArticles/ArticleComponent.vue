<template>
  <div class="article">
    <img
      v-if="article.imageTag == 'currency'"
      src="@/assets/images/image-currency.jpg"
      alt="Curreny Image"
      class="article__image"
    />
    <img
      v-if="article.imageTag == 'confetti'"
      src="@/assets/images/image-confetti.jpg"
      alt="Confetti Image"
      class="article__image"
    />
    <img
      v-if="article.imageTag == 'plane'"
      src="@/assets/images/image-plane.jpg"
      alt="Plane Image"
      class="article__image"
    />
    <img
      v-if="article.imageTag == 'restaurant'"
      src="@/assets/images/image-restaurant.jpg"
      alt="Restaurat Image"
      class="article__image"
    />
    <!-- <div :class="`article__image article__image--${article.imageTag}`"></div> -->
    <div class="article__text">
      <span class="article__text__author">By {{ article.author }}</span>
      <h4 class="article__text__title">{{ article.title }}</h4>
      <p class="article__text__description">{{ article.description }}</p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@import "@/assets/scss/_shared.scss";
.article {
  overflow: hidden;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: center;
  gap: 1.8rem;
  border-radius: 0.75rem;
  box-shadow: 0 2.4rem 4.8rem rgb(0 0 0 / 8%);
  &__image {
    width: 100%;
  }
  &__text {
    padding: 1rem 2rem 2.5rem 2rem;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: space-between;
    gap: 1.2rem;
    width: 95%;
    margin-inline: auto;
    &__author {
      color: $color-neutral-grayish-blue;
      font-size: 1.4rem;
    }
    &__title {
      color: $color-primary-dark-blue;
      font-weight: $font-weight-bold;
      line-height: 1.3;
    }
    &__description {
      font-size: 1.8rem;
      line-height: 1.2;
      font-weight: $font-weight-light;
      color: $color-neutral-grayish-blue;
    }
  }
}
</style>

<script>
export default {
  name: "ArticleComponent",
  data() {
    return {};
  },
  props: {
    article: {
      author: String,
      title: String,
      description: String,
      imageTag: String,
    },
  },
};
</script>
