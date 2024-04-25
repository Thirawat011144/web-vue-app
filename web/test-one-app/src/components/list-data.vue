<template>
  <div>
    {{ message }} {{ messageProp }} {{ post }}
    <person-data name="บีม" />
    <person-data name="โอด" />
  </div>
</template>

<script>
import personData from "./person-data.vue";
export default {
  name: "listData",
  data() {
    return {
      message: "รายชื่อพนักงาน",
    };
  },
  components: {
    personData,
  },
  props: {
    messageProp: {
      type: String,
      default: "",
    },
    post: { type: Object, default: "" },
  },
};
</script>

<style></style>
