<template>
  <div class="navigation">
    <img
      class="navigation__logo"
      src="@/assets/images/logo.svg"
      alt="Easybank Logo"
    />
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
  z-index: 250;
  display: flex;
  align-items: center;
  justify-content: space-between;
  background-color: $color-neutral-white;
  //padding: 1.5rem 0;
}
</style>
