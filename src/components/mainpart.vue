<template>
  <div class="comics-stuff">
    <img :src="img" alt="" />
    <h4>{{ series }}</h4>
  </div>
</template>

<script>
export default {
  name: "mainpart",
  props: {
    img: String,
    series: String,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.comics-stuff {
  padding: 10px;
  flex-basis: calc(100% / 6);
  cursor: pointer;

  img {
    width: 50%;
  }

  h4 {
    color: $main-text-color;
  }
}
</style>