<template>
  <Product
    v-for="product in products"
    :key="product.id"
    :product="product"
    class="product-item"
  >
  </Product>
</template>

<script>
import Product from "./Product.vue";
export default {
  name: "ProductList",
  props: {
    products: {
      type: Array,
      default: "",
    },
  },
  components: {
    Product,
  },
};
</script>

<style>
.title {
  font-size: 20px;
  color: aqua;
}
.p-q {
  font-size: 10px;
}
</style>
