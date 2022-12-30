<script setup>
import { storeToRefs } from "pinia";
import { useCounterStore } from "../stores/counter";
const store = useCounterStore();
const { count } = storeToRefs(store);
</script>

<template>
  <h2>ComponentC</h2>
  <div>{{ count }}</div>
</template>
