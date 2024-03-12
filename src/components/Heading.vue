<template>
  <h2>{{ headingMsg }}</h2>
</template>

<script setup>
defineProps({
  headingMsg: {
    type: String,
    default: "Content Title",
  },
});
</script>

<style scoped>
h2 {
  text-align: center;
  color: white;
}
</style>
