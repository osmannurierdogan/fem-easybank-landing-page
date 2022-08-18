<template>
  <button class="request-invite">Request Invite</button>
</template>

<script>
export default {
  name: "RequestInviteButton",
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/_shared.scss";
.request-invite {
  border-radius: 100px;
  padding: 1.5rem 2.5rem;
  border: none;
  outline: none;
  background: linear-gradient(
    90deg,
    $color-primary-lime-green,
    $color-primary-bright-cyan
  );
  color: $color-neutral-white;
  font-weight: $font-weight-bold;
  cursor: pointer;
  /* text-transform: uppercase;
  letter-spacing: 2px;
  font-size: 1.6rem; */
}
</style>
