<template>
  <header>
    <img src="../assets/img/dc-logo.png" alt="header-logo" />

    <headerlinks />
  </header>
</template>

<script>
import headerlinks from "./headerlinks.vue";

export default {
  components: {
    headerlinks,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

header {
  display: flex;
  height: 80px;
}
img {
  padding-left: 100px;
}
</style>