<script setup>
import { defineProps } from "vue";
const props = defineProps({
  firstName: {
    type: String,
    required: true,
    default: "not found",
  },
  lastName: {
    type: String,
    required: true,
    default: "not found",
  },
  age: {
    type: Number,
    required: true,
  },
});
</script>

<template>
  <div>
    <header>from props Validation</header>
    <h1>{{ firstName }}</h1>
    <p>{{ age }}</p>
    <hr />
    <h1>hello From un Validation Props {{ lastName }}</h1>
  </div>
</template>

<style scoped>
h1 {
  color: #333;
}
p {
  color: #666;
}
</style>
