<template>
  <div>
    <h1>B7</h1>
    <form action="">
      <input type="text" />
      <button @click="submit">Submit</button>
    </form>
  </div>
</template>

<script setup>
const submit = (event) => {
  event.preventDefault();

  console.log("Form submission prevented!");
};
</script>

<style></style>
