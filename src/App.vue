<!-- <template>
  <div>
    <p>binding property</p>
    <ul>
      <li>1. v-bind</li>
      <li>2. v-if, v-else-if</li>
      <li>3. v-show</li>
      <li>4. v-for</li>
      <li>5. v-model</li>
    </ul>
    <img :src="imgUrl" alt="" />
    <p v-bind:style="{ fontSize: size, color: red }">Text example</p>
    <p v-bind:class="className">V-bind Class</p>
    <p>
      Đối vs v-if thì điều kiện đúng sẽ render ra dom, nếu điều kiện sai sẽ ko
      render ra dom
    </p>
    <p>
      Còn đối vs v-show thì nếu điều kiện đúng hay sai thì element vx đc render
      ra dom, chỉ khác nếu điều kiện sai thì display:none
    </p>
    <p>v-if có thể kết hợp v-else</p>
    <ul>
      <li v-if="age > 30">Tuổi trung niên</li>
      <li v-else-if="age > 18">Tuổi trưởng thành</li>
      <li v-else-if="age > 10">Tuổi thiếu niên</li>
      <li v-else>Kid</li>
    </ul>

    <ul>
      <li v-for="student in sts">{{ student.name }}</li>
    </ul>

    <div>
      <input v-model="inputText" type="text" />
      <p>Gia tri ban nhap: {{ inputText }}</p>

      <input @input="handleChange" type="text" />
      <p>Gia tri ban nhap: {{ value }}</p>
    </div>

    <div>
      <button @click="handleClick('hello')">click</button>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
const imgUrl =
  "https://www.bing.com/th?id=OIP.jo0Mqph76elwG3j14m9vwgHaGq&w=146&h=132&c=8&rs=1&qlt=90&o=6&cb=13&dpr=1.5&pid=3.1&rm=2";

const size = "50px";
const red = "red";
const className = "custom-class";
const age = 20;
const sts = [
  { id: 1, name: "John Doe" },
  { id: 2, name: "Jane Doe" },
  { id: 3, name: "Mike Doe" },
];

const inputText = ref("he");

const value = ref("");

const handleChange = (event) => {
  console.log(event.target.value);
  value.value = event.target.value;
};

const handleClick = (message) => {
  console.log(message);
};
</script>

<style>
.custom-class {
  font-weight: bold;
  color: blue;
  font-size: 50px;
}
</style> -->

<template>
  <div>
    <Exercice01 />
    <Exercice02 />
    <Exercice03 />
    <Exercice04 />
    <Exercice05 />
    <Exercice06 />
    <Exercice07 />
    <Exercice08 />
    <Exercice09 />
    <Exercice10 />
    <Exercice11 />
    <Exercice12 />
  </div>
</template>

<script setup>
import Exercice01 from "./components/Exercise01.vue";
import Exercice02 from "./components/Exercise02.vue";
import Exercice03 from "./components/Exercise03.vue";
import Exercice04 from "./components/Exercise04.vue";
import Exercice05 from "./components/Exercise05.vue";
import Exercice06 from "./components/Exercise06.vue";
import Exercice07 from "./components/Exercise07.vue";
import Exercice08 from "./components/Exercise08.vue";
import Exercice09 from "./components/Exercise09.vue";
import Exercice10 from "./components/Exercise10.vue";
import Exercice11 from "./components/Exercise11.vue";
import Exercice12 from "./components/Exercise12.vue";
</script>

<style></style>
