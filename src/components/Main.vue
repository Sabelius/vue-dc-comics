<template>
  <main>
    <div class="main-title-container">
      <h1>-- CONTENT GOES HERE --</h1>
    </div>
    <section class="first-section">
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
              ><img
                src="../assets/img/buy-comics-merchandise.png"
                alt="merchbuy"
              />
              <h4>DC MERCHANDISE</h4></a
            >
          </li>
          <li>
            <a href=""
              ><img
                src="../assets/img/buy-comics-subscriptions.png"
                alt="subs"
              />
              <h4>SUBSCRIPTION</h4></a
            >
          </li>
          <li>
            <a href=""
              ><img
                src="../assets/img/buy-comics-shop-locator.png"
                alt="shop"
              />
              <h4>COMIC SHOP LOCATOR</h4></a
            >
          </li>
          <li>
            <a href=""
              ><img src="../assets/img/buy-dc-power-visa.svg" alt="visa" />
              <h4>DC POWER VISA</h4></a
            >
          </li>
        </ul>
      </nav>
    </section>

    <section class="second-section">
      <nav>
        <ul>
          <h3>DC COMICS</h3>
          <li><a href="">Characters</a></li>
          <li><a href="">Comics</a></li>
          <li><a href="">Movies</a></li>
          <li><a href="">Tv</a></li>
          <li><a href="">Games</a></li>
          <li><a href="">Video</a></li>
          <li><a href="">News</a></li>
          <ul class="magic-ul">
            <h3>SHOP</h3>
            <li><a href="">Shop DC</a></li>
            <li><a href="">Shop DC Collectibles</a></li>
          </ul>
        </ul>
        <ul>
          <h3>DC</h3>
          <li><a href="">Terms Of Use</a></li>
          <li><a href="">Privacy Policy(New)</a></li>
          <li><a href="">ad Choices</a></li>
          <li><a href="">Advertising</a></li>
          <li><a href="">Jobs</a></li>
          <li><a href="">Subscriptions</a></li>
          <li><a href="">Talent Work Shop</a></li>
          <li><a href="">CPSC Certificates</a></li>
          <li><a href="">Ratings</a></li>
          <li><a href="">Shop Help</a></li>
          <li><a href="">Contact Us</a></li>
        </ul>
        <ul>
          <h3>SITES</h3>
          <li><a href="">DC</a></li>
          <li><a href="">Mad Magazine</a></li>
          <li><a href="">DC Kids</a></li>
          <li><a href="">DC Universe</a></li>
          <li><a href="">DC Power Visa</a></li>
        </ul>
        <div>
          <img
            src="../assets/img/dc-logo-bg.png"
            alt="seond-main-section-img"
          />
        </div>
      </nav>
    </section>
  </main>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.main-title-container {
  background-color: $text-color;
  height: 100px;
  margin-top: 20px;
}
h1 {
  padding-top: 30px;
  padding-right: 1250px;
  color: $main-text-color;
}
.first-section {
  background-color: $main-buy-section-color;
  height: 130px;
}

.first-section ul {
  display: flex;
  justify-content: space-around;
  list-style: none;
  padding-top: 20px;
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
}
.second-section {
  background-image: url("../assets/img/footer-bg.jpg");
  height: 350px;
}
.second-section nav {
  display: flex;
}
.second-section ul {
  list-style: none;
  padding-left: 70px;
}
.second-section h3 {
  color: $main-text-color;
  padding-top: 25px;
}
.second-section li {
  padding-top: 5px;
}
.second-section a {
  text-decoration: none;
  color: $main-second-section-li;
}
.magic-ul {
  padding-right: 70px;
}
.second-section div{
    height: 350px;
    overflow: hidden;
}
.second-section img {
  width: 500px;
  margin-left: 400px;
}
</style>