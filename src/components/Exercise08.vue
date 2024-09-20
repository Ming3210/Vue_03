<template>
  <div>
    <h1>B8</h1>
    <a href="http://www.google.com" @click="checkLink"
      >Link 1: http://www.google.com</a
    ><br />

    <a href="https://www.google.com" @click="checkLink"
      >Link 2: https://www.google.com</a
    ><br />
  </div>
</template>

<script setup>
import { ref } from "vue";

const checkLink = (event) => {
  const url = event.target.getAttribute("href");

  if (!url.startsWith("https://")) {
    alert("Invalid Url");
    event.preventDefault();
  }
};
</script>

<style scoped>
a {
  margin-bottom: 10px;
  display: inline-block;
}
</style>
