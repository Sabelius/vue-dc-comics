<template>
  <main>
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