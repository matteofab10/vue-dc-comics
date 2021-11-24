<template>
  <header>
    <div class="container">
      <img src="../assets/img/dc-logo.png" alt="dc-logo">
      <ul>
        <li><a href="">characters</a></li>
        <li><a href="">comics</a></li>
        <li><a href="">movies</a></li>
        <li><a href="">tv</a></li>
        <li><a href="">games</a></li>
        <li><a href="">collectibles</a></li>
        <li><a href="">videos</a></li>
        <li><a href="">fans</a></li>
        <li><a href="">news</a></li>
        <li><a href="">shop</a></li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header"
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
          img {
            width: 80px;
          }
            li {
              list-style: none;
              display: inline-block;
              cursor: pointer;
            }
              a {
                text-decoration: none;
                color: black;
                padding: 15px;
                text-transform: uppercase;
                line-height: 96px;
              }
      }
  }

</style>