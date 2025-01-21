<script setup>
import { ref } from "vue";
let a = 10;
let data = ref(["Asif", "Fahim", "Naim", "Taif"]);
</script>

<template>
  <div>
    <h1>use of v-for</h1>
    <p v-for="(person, index) of data" :key="index">{{ person }}</p>
  </div>
</template>
