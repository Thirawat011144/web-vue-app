<template>
  <div>
    <p>App Component</p>
    <input type="text" v-model="message">
    <form-data />
    <list-data :messageProp="message" :post="post" />
  </div>
</template>

<script>
import listData from "./components/list-data.vue";
import formData from "./components/form-data.vue";

export default {
  name: "App",
  components: {
    listData,
    formData,
  },
  data() {
    return {
      message: "This is data.",
      post: {
        id: 1,
        title: "My  Journey vue",
      },
    };
  },
};
</script>

<style></style>
