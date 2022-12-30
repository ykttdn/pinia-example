<script setup>
const emit = defineEmits(["increment", "reset"]);
const increment = () => emit("increment");
const reset = () => emit("reset");
</script>

<template>
  <h2>Component B</h2>
  <button @click="increment">increment</button>
  <button @click="reset">reset</button>
</template>
