<script setup>
import { inject } from "vue";

const student = inject("student");
</script>

<template>
  <div>
    <h1>Student Component</h1>
    <p>{{ student.name }}</p>
    <p>{{ student.age }}</p>
    <p>{{ student.class }}</p>
  </div>
</template>
