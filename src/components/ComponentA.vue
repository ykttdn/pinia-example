<script setup>
const props = defineProps({
  count: Number,
});
</script>

<template>
  <h2>Component A</h2>
  <div>{{ props.count }}</div>
</template>
