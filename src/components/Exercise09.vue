<template>
  <div>
    <h1>B9</h1>
    <button @click="click">Click {{ count }} lần</button>
  </div>
</template>

<script setup>
import { ref } from "vue";

const count = ref(0);
const click = () => {
  count.value++;
};
</script>

<style></style>
