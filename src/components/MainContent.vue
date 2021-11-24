<template>
  <section>
    <div class="container">
      <div class="box">
        <img class="little-img" src="../assets/img/buy-comics-digital-comics.png" alt="digital-comics">
        <h4>digital comics</h4>
      </div>
      <div class="box">
        <img src="../assets/img/buy-comics-merchandise.png" alt="">
        <h4>dc merchandise</h4>
      </div>
      <div class="box">
        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
        <h4>subscriptions</h4>
      </div>
      <div class="box">
        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
        <h4>comic shop locator</h4>
      </div>
      <div class="box">
        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
        <h4>dc power visa</h4>
      </div>
    </div> 
  </section>
</template>

<script>
export default {
  name: "MainContent"
}
</script>

<style lang="scss">
  @import "../assets/style/vars.scss";

  section{
    background-color: $primary-color;
    display: flex;
    align-items: center;
    color: white;
    padding: 40px;
    .container {
      padding: 20px;
      display: flex;
      justify-content: space-between;
        .box {
          display: flex;
          align-items: center;
            img {
              width: 50px;
              margin-right: 5px;
            }
              h4 {
                font-size: 15px;
                text-transform: uppercase;
              }
                
        }
    }
  }

</style>