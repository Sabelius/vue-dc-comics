<template>
  <footer>
      <button>SIGN-UP NOW</button>
      <nav>
      <ul>
        <h2>FOLLOW US</h2>
        <li v-for="(link, index) in links" :key="index">
          <a><img :src="'./img/' + link.img" /></a>
        </li>
      </ul>
    </nav>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      links: [
        {
          img: "footer-facebook.png",
          url: "#",
        },
        {
          img: "footer-twitter.png",
          url: "#",
        },
        {
          img: "footer-youtube.png",
          url: "#",
        },
        {
          img: "footer-pinterest.png",
          url: "#",
        },
        {
          img: "footer-periscope.png",
          url: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

footer {
  background-color: $text-color;
  height: 127px;
}
button {
  background-color: $text-color;
  color: $main-text-color;
  padding: 20px;
  border-color: $main-text-color;
  margin-right: 1300px;
  margin-top: 25px;

  &:hover {
    border-color: $main-buy-section-color;
    cursor: pointer;
  }
}

ul {
  display: flex;
  padding-left: 1300px;
  margin-bottom: 100px;
}
ul h2 {
  color: $main-buy-section-color;
}
li {
  padding-left: 20px;
  list-style: none;
}
img {
  width: 30px;
  cursor: pointer;
}
</style>