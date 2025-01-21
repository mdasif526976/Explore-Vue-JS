<script setup>
const props = defineProps(["firstName", "lastName"]);
</script>
<template>
  <div>
    <h1>hello From Dynamic Props Component</h1>
    <h1>UserName:{{ firstName }} {{ lastName }}</h1>
  </div>
</template>
