<template>
  <header>
    <img src="../assets/img/dc-logo.png" alt="header-logo" />

    <nav>
      <ul>
        <li v-for= "(link, index) in links" :key= "index">
            <a :class= "{hover : link.value}">{{ link.text }}</a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
    name: 'Header',
    data: function(){
        return {
            links: [
                {
                    text:"CHARACTERS",
                    url: "#",
                    value:"true"
                },
                {
                    text:"COMICS",
                    url: "#",
                    value:"true"
                },
                {
                    text:"MOVIES",
                    url: "#",
                    value:"true"
                },
                {
                    text:"TV",
                    url: "#",
                    value:"true"
                },
                {
                    text:"GAMES",
                    url: "#",
                    value:"true"
                },
                {
                    text:"COLLECTIBLES",
                    url: "#",
                    value:"true"
                },
                {
                    text:"VIDEOS",
                    url: "#",
                    value:"true"
                },
                {
                    text:"FANS",
                    url: "#",
                    value:"true"
                },
                {
                    text:"NEWS",
                    url: "#",
                    value:"true"
                },
                {
                    text:"SHOPS",
                    url: "#",
                    value:"true"
                },
            ]
        }
    }
};
</script>

<style lang="scss" scoped>
header{
  display: flex;
}

ul {
  display: flex;
  list-style: none;
  padding-left: 700px;
}

li a{
    padding: 20px;
    vertical-align: middle;
    text-decoration: none;
    color: black;

    &:hover{
        color:blue;
        border-bottom: 3px solid blue;
        cursor: pointer;
    }
}
</style>