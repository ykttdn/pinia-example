<script setup>
import { ref } from "vue";
import ComponentA from "./ComponentA.vue";
import ComponentB from "./ComponentB.vue";

const count = ref(0);
const increment = () => {
  count.value++;
};
const reset = () => {
  count.value = 0;
};
</script>

<template>
  <h1>Vue</h1>
  <ComponentA :count="count"></ComponentA>
  <ComponentB @increment="increment" @reset="reset"></ComponentB>
</template>
