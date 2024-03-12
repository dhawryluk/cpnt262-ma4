<template>
  <button class="my-btn">
    <slot />
  </button>
</template>

<script setup></script>

<style scoped>
.my-btn {
  color: #fff;
  background-color: limegreen;
  border: none;
  padding: 6px;
  border-radius: 8px;
  cursor: pointer;
}

.my-btn:hover {
  box-shadow: 0 8px 8px 0 rgba(104, 255, 84, 0.2);
}
</style>
