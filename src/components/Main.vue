<template>
  <main>
    <div class="jumbotron">

    </div>
    <div class="container">
    </div>
  </main>
</template>

<script>
export default {
  name: "Main"
}
</script>

<style lang="scss">
  @import "../assets/style/vars.scss";


  main{
    .jumbotron {
      background-image: url('../assets/img/jumbotron.jpg');
      height: 400px;
    }
    .container{
      background-color: #1c1c1c;
      display: flex;
      align-items: center;
      color: white;
      h2 {
        font-weight: 600;
      }
    }
  }

</style>