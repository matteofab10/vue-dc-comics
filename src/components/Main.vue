<template>
  <main>
    <div class="jumbotron"></div>
    <div class="container heroBox">
      <div class="current-series">current series</div>
      <ProductCard 
        v-for="(product, index) in productItems"
        :key="index" 
        :product="product"
        />
      <div class="btn-series">
        <button>load more</button>
      </div>
    </div>
  </main>
</template>

<script>

import ProductCard from './ProductCard';
import productItems from '../assets/data/objectsData.js';

export default {
  name: "Main",
  components: {
    ProductCard
  },
  data(){
    return {
      productItems
    }
  }
}
</script>

<style lang="scss">
  @import "../assets/style/vars.scss";


  main{
    background-color: #1c1c1c;
    .jumbotron {
      background-image: url('../assets/img/jumbotron.jpg');
      height: 400px;
    }
    .heroBox {
      position: relative;
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      padding-top: 60px;
    }
    .current-series {
      position: absolute;
      top: -35px;
      left: -10px;
      padding: 10px 20px;
      background-color: #0282f9;
      color: white;
      text-transform: uppercase;
      font-size: 30px;
      font-weight: bold;
    }
    .btn-series {
      display: flex;
      justify-content: center;
      width: 100%;
    }
    button {
      background-color: #0282f9;
      color: white;
      padding: 15px 70px;
      cursor: pointer;
      text-transform: uppercase;
      margin: 30px 0;
      border: none;
      font-weight: bold;
    }
  }

</style>