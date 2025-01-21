<script setup>
import { reactive, ref } from "vue";
// its only for premitive data type
let initialState = reactive({ val: { user: ["Md Asif"], count: 0 } });
const addUser = () => {
  initialState.val.user.push("Md Fahim");
};
// reactive can store ref
const value = reactive(ref("Asif"), ref("Fahim"));
</script>
<template>
  <div>
    <h1>My Reactive Page</h1>
    <h1>UserName:{{ initialState.val.user }}</h1>
    <p>{{ initialState.val.count }}</p>
    <button @click="initialState.val.count++">+</button>
    <button v-on:click="addUser">Add User</button>
  </div>
</template>
