<template>
  <main>
    <div class="main-title-container">
    <h1>-- CONTENT GOES HERE --</h1>
    </div>
    <section class="first-section">
        <nav>
            <ul>
                <li><a href=""><img src="../assets/img/buy-comics-digital-comics.png" alt="comicsbuy"><h4>DIGITAL COMICS</h4></a></li>
                <li><a href=""><img src="../assets/img/buy-comics-merchandise.png" alt="merchbuy"><h4>DC MERCHANDISE</h4></a></li>
                <li><a href=""><img src="../assets/img/buy-comics-subscriptions.png" alt="subs"><h4>SUBSCRIPTION</h4></a></li>
                <li><a href=""><img src="../assets/img/buy-comics-shop-locator.png" alt="shop"><h4>COMIC SHOP LOCATOR</h4></a></li>
                <li><a href=""><img src="../assets/img/buy-dc-power-visa.svg" alt="visa"><h4>DC POWER VISA</h4></a></li>
            </ul>
        </nav>
    </section>

    <section class="second-section"></section>
  </main>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.main-title-container{
  background-color: $text-color;
  height: 100px;
  margin-top: 20px;
}
h1{
    padding-top: 30px;
    padding-right: 1250px;
    color: $main-text-color;
}
.first-section{
    background-color: $main-buy-section-color;
    height: 130px;
}

ul{
    display: flex;
    justify-content: space-around;
    list-style: none;
    padding-top: 20px;
}
img{
    width: 60px;
}
a{
    color: $main-text-color;
    text-decoration: none;
    display: flex;
}
h4{
    padding: 30px 0 0 10px;
}
.second-section{
    background-image: url("../assets/img/footer-bg.jpg");
    height: 350px;

}

</style>