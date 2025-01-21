<script setup>
import { ref } from "vue";

const formData = ref({ userName: "", email: "", password: "" });
const handleSubmit = () => {
  console.log(formData.value);
};
</script>

<template>
  <form @submit.prevent>
    <input
      type="text"
      v-model="formData.userName"
      placeholder="Enter your user name"
    />
    <input
      type="text"
      v-model="formData.email"
      placeholder="Enter your email"
    />
    <input
      type="text"
      v-model="formData.password"
      placeholder="Enter your password"
    />
    <button type="submit" @click="handleSubmit">Submit</button>
  </form>
</template>
