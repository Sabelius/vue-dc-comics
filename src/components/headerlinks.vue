<template>
  <nav>
    <ul>
      <li v-for="(link, index) in links" :key="index">
        <a :class="{ hover: link.value }">{{ link.text }}</a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "headerlinks",
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
          text: "COLLECTIBLES",
          url: "#",
          value: "true",
        },
        {
          text: "VIDEOS",
          url: "#",
          value: "true",
        },
        {
          text: "FANS",
          url: "#",
          value: "true",
        },
        {
          text: "NEWS",
          url: "#",
          value: "true",
        },
        {
          text: "SHOPS",
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

ul {
  display: flex;
  list-style: none;
  padding-left: 400px;
  padding-top: 40px;
}

li a {
  padding: 20px;
  text-decoration: none;
  color: $text-color;

  &:hover {
    color: $main-buy-section-color;
    border-bottom: 3px solid $main-buy-section-color;
    cursor: pointer;
  }
}
</style>