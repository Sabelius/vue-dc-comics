<template>
  <main>
    <mainpart />
    <section class="first-section">
      <mainfirstsection />
    </section>

    <section class="second-section">
      <mainsecondsection />
    </section>
  </main>
</template>

<script>
import mainpart from "./mainpart.vue";
import mainfirstsection from "./mainfirstsection.vue";
import mainsecondsection from "./mainsecondsection.vue";

export default {
  components: {
    mainpart,
    mainfirstsection,
    mainsecondsection,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.first-section {
  background-color: $main-buy-section-color;
  height: 130px;
}
.second-section {
  background-image: url("../assets/img/footer-bg.jpg");
}
</style>