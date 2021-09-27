<template>
  <main>
    <div class="jumbotron">
      <div class="series-title-container"><h3>CURRENT SERIES</h3></div>
    </div>
    <div class="container-comics">
      <mainpartsenior />
    </div>
    <section class="first-section">
      <mainfirstsection />
    </section>

    <section class="second-section">
      <mainsecondsection />
    </section>
  </main>
</template>

<script>
import mainpartsenior from "./mainpartsenior.vue";
import mainfirstsection from "./mainfirstsection.vue";
import mainsecondsection from "./mainsecondsection.vue";

export default {
  name: "Main",
  components: {
    mainpartsenior,
    mainfirstsection,
    mainsecondsection,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.jumbotron{
  background-image: url("../assets/img/jumbotron.jpg");
  height: 400px;
  display: flex;
}
.series-title-container{
  height: 30px;
  width: 200px;
  background-color: $main-buy-section-color;
  align-self: flex-end;
  margin-top: 200px;
  margin-left: 300px;
  display: flex;
}
h3{
  color: $main-text-color;
  align-self: center;
  margin-left: 15px;
}
.container-comics {
  background-color: $text-color;
}

.first-section {
  background-color: $main-buy-section-color;
}

.second-section {
  background-image: url("../assets/img/footer-bg.jpg");
}
</style>