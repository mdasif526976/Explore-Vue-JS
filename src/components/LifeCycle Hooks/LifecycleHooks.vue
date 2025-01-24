<script setup>
import {
  onBeforeMount,
  onMounted,
  onBeforeUpdate,
  onUpdated,
  onBeforeUnmount,
  onUnmounted,
  ref,
} from "vue";
const message = ref("Hello Vue 3");

const update = () => (message.value = "Hello Vue 3 Updated");

onBeforeMount(() => {
  console.log("component before mount");
});

onMounted(() => {
  console.log("component mounted");
});

onUpdated(() => {
  console.log("component updated");
});
onBeforeUnmount(() => {
  console.log("component before unmount");
});
onUnmounted(() => {
  console.log("component unmounted");
});
</script>

<template>
  <div>
    <h1>LifeCycle Hooks</h1>
    <p>{{ message }}</p>
    <button @click="update">Update</button>
  </div>
</template>
