<template>
  <div class="product-card">
    <img :src="product.thumb" :alt="product.series">
    <h3>{{product.series}}</h3>
  </div>
</template>

<script>
export default {
  name: 'ProductCard',
  props: {
    product: Object,
  }
}
</script>

<style lang="scss">
  @import "../assets/style/vars.scss";

  .product-card {
    width: calc(100% / 6);
    padding: 10px;
    img {
      object-fit: cover;
      object-position: top;
      width: 100%;
      height: 170px;
    }
    h3 {
      color: white;
    }
  }
</style>