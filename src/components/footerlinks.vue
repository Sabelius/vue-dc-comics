<template>
  <nav>
    <ul>
      <h2>FOLLOW US</h2>
      <li v-for="(link, index) in links" :key="index">
        <a><img :src="'./img/' + link.img" /></a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "footerlinks",
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