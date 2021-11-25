<template>
  <header>
    <div class="container">
      <img src="../assets/img/dc-logo.png" alt="dc-logo">
      <ul>
        <li
        v-for="(link, index) in links" 
        :key="`nav-top${index}`"
        :class="{active : (index === counter)}">
        <a
        class="nav-list-border"
        href="#">{{link.text}}</a></li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",

  data(){
    return{
      links: [
        {
          url: "/characters",
          text: "characters",
          active: false
        },
        {
          url: "/comics",
          text: "comics",
          active: false 
        },
        {
          url: "/movies",
          text: "movies",
          active: false
        },
        {
          url: "/tv",
          text: "tv",
          active: false
        },
        {
          url: "/games",
          text: "games",
          active: false
        },
        {
          url: "/collectibles",
          text: "collectibles",
          active: false
        },
        {
          url: "/videos",
          text: "videos",
          active: false
        },
        {
          url: "/fans",
          text: "fans",
          active: false
        },
        {
          url: "/news",
          text: "news",
          active: false
        },
        {
          url: "/shop",
          text: "shop",
          active: false
        },
      ],
      counter: 1,
    }
  }
}
</script>

<style lang="scss">
  @import "../assets/style/vars.scss";

  header {
    height: 100px;
      .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
          li {
            list-style: none;
            display: inline-block;
            cursor: pointer;
            &:hover a {
              color: $primary-color;
            }
            &:hover,
            &.active {
              border-bottom: 4px solid $primary-color;
            }
            &.active a {
              color: $primary-color;
            }
            a {
              text-decoration: none;
              color: black;
              padding: 15px;
              text-transform: uppercase;
              line-height: 96px;
            }
          }
          img {
            width: 70px;
            cursor: pointer;
          }
          .nav-list-border {
            line-height: 96px;
          }
      }
  }

</style>