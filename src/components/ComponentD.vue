<script setup>
import { useCounterStore } from "../stores/counter";
const store = useCounterStore();
const { increment, reset } = store;
</script>

<template>
  <h2>ComponentD</h2>
  <button @click="increment">increment</button>
  <button @click="reset">reset</button>
</template>
