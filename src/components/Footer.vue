<template>
  <footer>
    <div>
      <button>SIGN-UP NOW</button>
    </div>
    <nav>
        <h2>FOLLOW US</h2>
        <ul>
            <li><a href=""><img src="" alt=""></a></li>
            <li><a href=""><img src="" alt=""></a></li>
            <li><a href=""><img src="" alt=""></a></li>
            <li><a href=""><img src="" alt=""></a></li>
        </ul>
    </nav>
  </footer>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

footer {
  background-color: $text-color;
  height: 174px;
}
div {
  padding: 40px 1200px 0 0;
}
button {
  background-color: $text-color;
  color: white;
  padding: 20px;
  border-color: $main-text-color;

  &:hover {
    border-color: $main-buy-section-color;
    cursor: pointer;
  }
}
</style>