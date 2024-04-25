<template>
  <div>
    <p>ชื่อ {{ name }}</p>
   
  </div>
</template>

<script>
export default {
  name: "personData",
  data() {
    return {
      message: "ชื่อ-นามสกุล",
    };
  },
  props: ["name"],
  created() {
    console.log(this.name);
  },
};
</script>

<style></style>
