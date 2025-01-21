<script setup>
import { computed, ref } from "vue";
const counter = ref(0);
const squere = computed(() => {
  return counter.value ** 2;
});
console.log(squere);
</script>

<template>
  <div>
    <h1>from computed properties Page</h1>
    <p>Count:{{ counter }}</p>
    <p>Squre Value: {{ squere }}</p>
    <button @click="counter++">Increament</button>
  </div>
</template>
