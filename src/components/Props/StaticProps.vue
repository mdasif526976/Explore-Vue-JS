<script setup>
let name = defineProps(["user"]);
</script>
<template>
  <div>
    <h1>hello From Static Props Component</h1>
    <h2>{{ name.user }}</h2>
  </div>
</template>
