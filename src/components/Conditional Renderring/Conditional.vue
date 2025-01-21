<script setup>
import { ref } from "vue";

let isTrue = false;
let isFalse = true;
let show = ref(true);
</script>

<template>
  <h1>hi from Conditional Renderring Page</h1>
  <p v-if="isTrue">Show this teg if 1st condition true</p>
  <p v-else-if="isFalse">Show this teg if 2nd condition true</p>

  <p v-else>Show this teg if else condition true</p>
  <p v-if="show">Hi I am asif</p>
  <button @click="show = !show">
    Click to <span v-if="show">hide</span
    ><span v-else-if="!show">Show</span> Content
  </button>
</template>
