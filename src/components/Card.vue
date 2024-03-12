<template>
  <div class="card">
    <img
      class="cardImage"
      src="../assets/pexels-pixabay-163036.jpg"
      alt="mario bros"
    />
    <Heading :headingMsg="headingMsg" />
    <myButton @click="toggleDropdown"> Read More </myButton>
    <div v-if="dropdownVisible">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dolorem quis
        blanditiis dolore. Cum placeat facilis quae consectetur excepturi,
        quidem, necessitatibus et quibusdam animi accusantium rem saepe
        reiciendis odit laudantium magnam.
      </p>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
import Heading from "./Heading.vue";
import myButton from "./myButton.vue";

const dropdownVisible = ref(false);

function toggleDropdown() {
  dropdownVisible.value = !dropdownVisible.value;
}
</script>

<style scoped>
.card {
  display: flex;
  flex-direction: column;
  max-width: 250px;
  background-color: rgb(26, 26, 26);
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.3);
  padding-bottom: 16px;
  margin: 20px;
  border-radius: 8px;
}

.cardImage {
  width: 100%;
  background-position: center;
}

.heading {
  font-size: 16px;
  margin: 20px;
}
</style>
