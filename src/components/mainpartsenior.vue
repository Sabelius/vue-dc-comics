<template>
  <div class="comics-part">
    <mainpart
      v-for="(link, index) in links"
      :key="index"
      :img="link.thumb"
      :series="link.series"
    />
    <div><button>LOAD MORE</button></div>
  </div>
</template>

<script>
import mainpart from "./mainpart.vue";
import json from "./json/dc-comics.json"

export default {
  name: "mainpartsenior",
  props: ["thumb", "series"],
  components: {
    mainpart,
  },
  data() {
    return {
      links: json
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.comics-part {
  margin: 0 auto;
  display: flex;
  flex-wrap: wrap;
  width: 70%;
  background-color: $text-color;
}
div {
  justify-content: center;
  padding: 5px;
}
button {
  font-size: 15px;
  background-color: $main-buy-section-color;
  color: $main-text-color;
  padding: 5px;
  border: none;
  cursor: pointer;
}
</style>