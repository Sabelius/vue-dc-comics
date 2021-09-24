<template>
  <main>
    <div class="main-title-container">
      <h1>- - CONTENT GOES HERE - -</h1>
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
                <img
                  src="../assets/img/buy-comics-subscriptions.png"
                  alt="subs"
                />
              </div>
              <h4>SUBSCRIPTION</h4></a
            >
          </li>
          <li>
            <a href="">
              <div>
                <img
                  src="../assets/img/buy-comics-shop-locator.png"
                  alt="shop"
                />
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
    </section>

    <section class="second-section">
      <nav>
        <ul class="second-ul">
          <h3>DC COMICS</h3>
          <li v-for="(link, index) in links" :key="index">
            <a>{{ link.text }}</a>
          </li>
          <ul>
            <h3>SHOP</h3>
            <li v-for="(link2, index) in links2" :key="index">
              <a>{{ link2.text }}</a>
            </li>
          </ul>
        </ul>
        <ul class="second-ul">
          <h3>DC</h3>
          <li v-for="(link3, index) in links3" :key="index">
            <a>{{ link3.text }}</a>
          </li>
        </ul>
        <ul class="second-ul">
          <h3>SITES</h3>
          <li v-for="(link4, index) in links4" :key="index">
            <a>{{ link4.text }}</a>
          </li>
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
export default {
  name: "Main",
  data() {
    return {
      links: [
        {
          text: "CHARACTERS",
          url: "#",
        },
        {
          text: "COMICS",
          url: "#",
        },
        {
          text: "MOVIES",
          url: "#",
        },
        {
          text: "TV",
          url: "#",
        },
        {
          text: "GAMES",
          url: "#",
        },
        {
          text: "VIDEO",
          url: "#",
        },
        {
          text: "NEWS",
          url: "#",
        },
      ],
      links2: [
        {
          text: "SHOP DC",
          url: "#",
        },
        {
          text: "SHOP DC COLLECTIBLES",
          url: "#",
        },
      ],
      links3: [
        {
          text: "Terms Of Use",
          url: "#",
        },
        {
          text: "Privacy Policy(New)",
          url: "#",
        },
        {
          text: "Ad Choices",
          url: "#",
        },
        {
          text: "Advertising",
          url: "#",
        },
        {
          text: "Jobs",
          url: "#",
        },
        {
          text: "Subscriptions",
          url: "#",
        },
        {
          text: "Talent Work Shop",
          url: "#",
        },
        {
          text: "CPSC Certificates",
          url: "#",
        },
        {
          text: "Ratings",
          url: "#",
        },
        {
          text: "Shop Help",
          url: "#",
        },
        {
          text: "Contact Us",
          url: "#",
        },
      ],
      links4: [
        {
          text: "DC",
          url: "#",
        },
        {
          text: "Mad Magazine",
          url: "#",
        },
        {
          text: "DC Kids",
          url: "#",
        },
        {
          text: "DC Universe",
          url: "#",
        },
        {
          text: "DC Power Visa",
          url: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.main-title-container {
  background-color: $text-color;
  height: 120px;
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
.first-section div{
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
.second-section {
  background-image: url("../assets/img/footer-bg.jpg");
}
.second-section nav {
  display: flex;
}
.second-ul {
  list-style: none;
  padding-left: 70px;
  text-align: left;
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
  cursor: pointer;

  &:hover {
    border-bottom: 1px solid $main-text-color;
  }
}
.second-section div {
  height: 400px;
  overflow: hidden;
}
.second-section img {
  width: 500px;
  margin-left: 400px;
}
</style>