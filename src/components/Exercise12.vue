<template>
  <div>
    <h1>B12</h1>
    <img :src="currentImage" alt="Random Image" width="300" height="200" />

    <button @click="changeImage">Change image</button>
  </div>
</template>

<script setup>
import { ref } from "vue";

const images = [
  "https://pbs.twimg.com/profile_images/1656466923/Article330142_armor_games_logo.jpg",
  "https://th.bing.com/th/id/OIP.NQbXJLoJ12znpsFoFYCwPAHaFj?rs=1&pid=ImgDetMain",
  "https://th.bing.com/th/id/OIP.sdTcs-u_PTJyakgDe0kOWAHaHa?rs=1&pid=ImgDetMain",
  "https://th.bing.com/th/id/R.516f9283cc5733db80d75126ac1f87d8?rik=B7zeg9m38K4tkA&pid=ImgRaw&r=0",
];

const currentImage = ref(images[0]);

const changeImage = () => {
  const randomIndex = Math.floor(Math.random() * images.length);
  currentImage.value = images[randomIndex];
};
</script>

<style scoped>
button {
  display: block;
  margin-top: 20px;
  padding: 10px 20px;
  font-size: 16px;
}

img {
  width: 200px;
  height: auto;
}
</style>
