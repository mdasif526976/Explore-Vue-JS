<script setup>
import { ref } from "vue";

let count = ref(0);
</script>
<template>
  <header>This page for Events</header>
  <h1>Count:{{ count }}</h1>
  <button type="" v-on:click="count++">increment</button>
  <!-- also you can use -->
  <button @click="count++">Decrement</button>
</template>
