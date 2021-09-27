<template>
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
      <img src="../assets/img/dc-logo-bg.png" alt="second-main-section-img" />
    </div>
  </nav>
</template>

<script>
export default {
  name: "mainsecondsection",
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