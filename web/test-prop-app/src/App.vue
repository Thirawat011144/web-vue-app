<template>
  <div>
    <h2>สวัสดี</h2>
    <h2>โปรแกรมแสดงรายการสินค้าที่ต้องการขาย</h2>
    <product-list :products="product" />
  </div>
</template>

<script>
import ProductList from "./components/ProductList.vue";

export default {
  name: "App",
  components: {
    ProductList,
  },
  data() {
    return {
      product: [
        { id: 1, name: "Keyboard", price: 500, quantity: 10 },
        { id: 2, name: "Mouse", price: 300, quantity: 3 },
        { id: 3, name: "Monitor", price: 2000, quantity: 2 },
        { id: 4, name: "Headphones", price: 1000, quantity: 7 },
      ],
    };
  },
};
</script>

<style></style>
