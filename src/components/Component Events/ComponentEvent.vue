<script setup>
import { ref } from "vue";
import ChildComponent from "./ChildComponent.vue";
import FromEvent from "./FromEvent.vue";
let count = ref(0);
const handleSubmit = (data) => {
  console.log("name", data.name);
  console.log("email", data.email);
};
</script>
<template>
  <div>
    <h1>Component Event</h1>
    <p>{{ count }}</p>
    <ChildComponent @increment="count++" />
    <hr />
    <header>Lets start Form Events</header>
    <FromEvent @userInfo="handleSubmit" />
  </div>
</template>
