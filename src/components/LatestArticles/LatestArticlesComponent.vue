<template>
  <section class="section--light-gray">
    <div class="container">
      <div class="articles">
        <h2 class="title">Latest Articles</h2>
        <div class="article-box">
          <ArticleComponent
            v-for="article in articles"
            :key="article"
            :article="article"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import ArticleComponent from "@/components/LatestArticles/ArticleComponent.vue";
export default {
  name: "LatestArticlesComponent",
  components: {
    ArticleComponent,
  },
  data() {
    return {
      articles: [
        {
          title: "Receive money in any currency with no fees",
          author: "Claire Robinson",
          description:
            "The world is getting smaller and we’re becoming more mobile. So why should you be forced to only receive money in a single …",
          imageTag: "currency",
        },
        {
          title: "Treat yourself without worrying about money",
          author: "Wilson Hutton",
          description:
            "Our simple budgeting feature allows you to separate out your spending and set realistic limits each month. That means you …",
          imageTag: "restaurant",
        },
        {
          title: "Take your Easybank card wherever you go",
          author: "Wilson Hutton",
          description:
            "We want you to enjoy your travels. This is why we don’t charge any fees on purchases while you’re abroad. We’ll even show you …",
          imageTag: "plane",
        },
        {
          title: "Our invite-only Beta accounts are now live!",
          author: "Claire Robinson",
          description:
            "After a lot of hard work by the whole team, we’re excited to launch our closed beta. It’s easy to request an invite through the site ...",
          imageTag: "confetti",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/_shared.scss";
.articles {
  padding: 6.4rem 0 7.4rem;
}
.title {
  font-weight: $font-weight-regular;
  font-size: 3.6rem;
  color: $color-primary-dark-blue;
  margin-bottom: 4.8rem;
}
.article-box {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  gap: 2.4rem;
}
</style>
