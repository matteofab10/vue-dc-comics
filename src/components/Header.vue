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
          text: "characters",
          active: false
        },
        {
          text: "comics",
          active: false 
        },
        {
          text: "movies",
          active: false
        },
        {
          text: "tv",
          active: false
        },
        {
          text: "games",
          active: false
        },
        {
          text: "collectibles",
          active: false
        },
        {
          text: "videos",
          active: false
        },
        {
          text: "fans",
          active: false
        },
        {
          text: "news",
          active: false
        },
        {
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