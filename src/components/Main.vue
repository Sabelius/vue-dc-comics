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
            <a href="">
              <img
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
          <li v-for="(link, index) in links" :key="index">
            <a>{{ link.text }}</a>
          </li>
          <ul class="magic-ul">
            <h3>SHOP</h3>
            <li v-for="(link2, index) in links2" :key="index">
              <a>{{ link2.text }}</a>
            </li>
          </ul>
        </ul>
        <ul>
          <h3>DC</h3>
          <li v-for="(link3, index) in links3" :key="index">
            <a>{{ link3.text }}</a>
          </li>
        </ul>
        <ul>
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
          value: "true",
        },
        {
          text: "COMICS",
          url: "#",
          value: "true",
        },
        {
          text: "MOVIES",
          url: "#",
          value: "true",
        },
        {
          text: "TV",
          url: "#",
          value: "true",
        },
        {
          text: "GAMES",
          url: "#",
          value: "true",
        },
        {
          text: "VIDEO",
          url: "#",
          value: "true",
        },
        {
          text: "NEWS",
          url: "#",
          value: "true",
        },
      ],
      links2: [
        {
          text: "SHOP DC",
          url: "#",
          value: "true",
        },
        {
          text: "SHOP DC COLLECTIBLES",
          url: "#",
          value: "true",
        },
      ],
      links3: [
        {
          text: "Terms Of Use",
          url: "#",
          value: "true",
        },
        {
          text: "Privacy Policy(New)",
          url: "#",
          value: "true",
        },
        {
          text: "Ad Choices",
          url: "#",
          value: "true",
        },
        {
          text: "Advertising",
          url: "#",
          value: "true",
        },
        {
          text: "Jobs",
          url: "#",
          value: "true",
        },
        {
          text: "Subscriptions",
          url: "#",
          value: "true",
        },
        {
          text: "Talent Work Shop",
          url: "#",
          value: "true",
        },
        {
          text: "CPSC Certificates",
          url: "#",
          value: "true",
        },
        {
          text: "Ratings",
          url: "#",
          value: "true",
        },
        {
          text: "Shop Help",
          url: "#",
          value: "true",
        },
        {
          text: "Contact Us",
          url: "#",
          value: "true",
        },
      ],
      links4: [
        {
          text: "DC",
          url: "#",
          value: "true",
        },
        {
          text: "Mad Magazine",
          url: "#",
          value: "true",
        },
        {
          text: "DC Kids",
          url: "#",
          value: "true",
        },
        {
          text: "DC Universe",
          url: "#",
          value: "true",
        },
        {
          text: "DC Power Visa",
          url: "#",
          value: "true",
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
.second-section div {
  height: 350px;
  overflow: hidden;
}
.second-section img {
  width: 500px;
  margin-left: 400px;
}
</style>