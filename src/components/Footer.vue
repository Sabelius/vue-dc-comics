<template>
  <footer>
    <button>SIGN-UP NOW</button>
    <footerlinks />
  </footer>
</template>

<script>
import footerlinks from "./footerlinks.vue";

export default {
  components: {
    footerlinks,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

footer {
  background-color: $text-color;
  height: 127px;
}
button {
  background-color: $text-color;
  color: $main-text-color;
  padding: 20px;
  border-color: $main-text-color;
  margin-right: 1300px;
  margin-top: 25px;

  &:hover {
    border-color: $main-buy-section-color;
    cursor: pointer;
  }
}
</style>