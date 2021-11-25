<template>
  <main>
    <div class="jumbotron"></div>

    <div class="container heroBox">

      <ProductCard 
        v-for="(product, index) in productItems"
        :key="index" 
        :product="product"
        />

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
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
    }
  }

</style>