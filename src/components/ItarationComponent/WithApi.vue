<template>
  <div>
    <h1>V-for with api</h1>
    <div v-for="comment in data" :key="comment.id">
      <p>id:{{ comment.id }}</p>
      <p>name:{{ comment.name }}</p>
      <p>email:{{ comment.email }}</p>
      <p>body:{{ comment.body }}</p>
      <button @click="userData(comment.name)">user</button>
    </div>
    <button @click="LoadData">LoadData</button>
  </div>
</template>

<script setup>
import { ref } from "vue";

const url = "https://jsonplaceholder.typicode.com/comments";
const data = ref([]);
// const fetch = async () => {
//   try {
//     const response = await fetch(url);
//     if (!response.ok) {
//       throw new Error("Network response not ok");
//     }
//     data.value = await response.json();
//   } catch (err) {
//     console.log(err);
//   }
// };
const LoadData = () => {
  fetch("https://jsonplaceholder.typicode.com/comments")
    .then((res) => res.json())
    .then((datas) => (data.value = datas))
    .catch((err) => console.log(err));
};
const userData = (user) => {
  console.log(user);
};

console.log(data);
</script>
