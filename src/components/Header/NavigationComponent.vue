<template>
  <div class="navigation">
    <img class="navigation__logo" src="@/assets/images/logo.svg" alt="" />
    <NavigationList />
    <RequestInviteButton />
  </div>
</template>

<script>
import RequestInviteButton from "@/components/Shared/RequestInviteButton.vue";
import NavigationList from "@/components/Header/NavigationList.vue";
export default {
  name: "NavigationComponent",
  components: {
    RequestInviteButton,
    NavigationList,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/_shared.scss";
.navigation {
  position: relative;
  z-index: 999;
  display: flex;
  align-items: center;
  justify-content: space-between;
  background-color: $color-neutral-white;
  padding: 1.5rem auto;
}
</style>
