<template>
  <nav>
    <ul>
      <li>
        <a href=""
          ><img
            src="../assets/img/buy-comics-digital-comics.png"
            alt="comicsbuy"
          />
          <h4>DIGITAL COMICS</h4></a
        >
      </li>
      <li>
        <a href=""
          ><div>
            <img
              src="../assets/img/buy-comics-merchandise.png"
              alt="merchbuy"
            />
          </div>
          <h4>DC MERCHANDISE</h4></a
        >
      </li>
      <li>
        <a href="">
          <div>
            <img src="../assets/img/buy-comics-subscriptions.png" alt="subs" />
          </div>
          <h4>SUBSCRIPTION</h4></a
        >
      </li>
      <li>
        <a href="">
          <div>
            <img src="../assets/img/buy-comics-shop-locator.png" alt="shop" />
          </div>
          <h4>COMIC SHOP LOCATOR</h4></a
        >
      </li>
      <li>
        <a href="">
          <div>
            <img src="../assets/img/buy-dc-power-visa.svg" alt="visa" />
          </div>
          <h4>DC POWER VISA</h4></a
        >
      </li>
    </ul>
  </nav>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.first-section ul {
  display: flex;
  justify-content: space-around;
  list-style: none;
  padding-top: 20px;
}
.first-section div {
  display: flex;
  vertical-align: middle;
}
img {
  width: 60px;
}
.first-section a {
  color: $main-text-color;
  text-decoration: none;
  display: flex;
}
h4 {
  padding: 30px 0 0 10px;
  cursor: pointer;
}
</style>