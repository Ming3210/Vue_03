<template>
  <div>
    <h1>B4</h1>
    <ul>
      <li v-if="active == true" class="active">Block</li>
      <li v-else class="disActive">Blocked</li>
    </ul>
    <button @click="pop">click</button>
  </div>
</template>

<script setup>
import { ref } from "vue";
const active = ref(true);

const pop = () => {
  active.value = !active.value;
  console.log(active.value); // Log the value
};
</script>

<style>
.active {
  background-color: blue;
  color: white;
  padding: 10px;
  border-radius: 5px;
  margin-bottom: 10px;
  transition: background-color 0.3s ease;
}
.disActive {
  background-color: rgb(255, 0, 0);
  color: rgb(0, 0, 0);
  padding: 10px;
  border-radius: 5px;
  margin-bottom: 10px;
  transition: background-color 0.3s ease;
}
</style>
