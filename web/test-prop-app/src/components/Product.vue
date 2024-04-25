<template>
  <div :key="product.id">
    <div class="title">{{ product.name }}</div>
    <div class="p-q">{{ product.price }}</div>
    <div class="p-q">{{ product.quantity }}</div>
  </div>
</template>

<script>
export default {
  name: "Product",
  props: {
    product: {
      type: Object,
      default: "",
    },
  },
};
</script>

<style></style>
