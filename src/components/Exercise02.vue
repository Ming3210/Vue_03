<template>
  <div id="app" data-v-app>
    <h1>B2</h1>
    <h1 v-bind:id="elementId" v-bind:class="elementClass">Heading</h1>
  </div>
</template>

<script setup>
const elementId = "heading";
const elementClass = "heading";
</script>

<style></style>
