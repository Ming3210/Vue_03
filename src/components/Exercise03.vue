<template>
  <div>
    <h1>B3</h1>
    <ul>
      <li v-if="isDisabled == true"><input type="text" disabled /></li>
      <li v-else><input type="text" placeholder="Cho phép nhập" /></li>
    </ul>
  </div>
</template>

<script setup>
const isDisabled = false;
</script>

<style>
ul {
  list-style-type: none;
  padding: 0;
}
</style>
