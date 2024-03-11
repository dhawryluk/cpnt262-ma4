<script setup>
import Card from "./components/Card.vue";
// import { ref } from "vue";
</script>

<template>
  <div id="app">
    <h2 v-bind:id="headingId">Learning Vue!</h2>
    <Card />
  </div>
</template>

<style scoped></style>
