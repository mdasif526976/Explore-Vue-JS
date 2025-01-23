<script setup>
import { reactive } from "vue";
const userInfo = reactive({
  name: "",
  email: "",
});
</script>

<template>
  <div>
    <form @submit.prevent="$emit('userInfo', userInfo)">
      <label for="name">Name:</label>
      <input type="text" id="name" v-model="userInfo.name" />

      <label for="email">Email:</label>
      <input type="email" id="email" v-model="userInfo.email" />

      <button type="submit">Submit</button>
    </form>
  </div>
</template>
