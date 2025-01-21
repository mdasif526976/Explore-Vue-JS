<script setup>
const submitHandler = (event) => {
  event.preventDefault();
  const name = event.target.name.value;
  const email = event.target.email.value;
  console.log(name, email);
};
</script>

<template>
  <h1>hi from input</h1>
  <form @submit="submitHandler">
    <input id="name" type="text" placeholder="enter your name" />
    <input id="email" type="email" placeholder="wnter your email" />
    <button type="submit">Submit</button>
  </form>
</template>
