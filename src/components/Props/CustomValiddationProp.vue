<script setup>
defineProps({
  name: {
    type: String,
    required: true,
    validator: (propsValue) => (propsValue ? true : false),
  },
  age: {
    type: Number,
    required: true,
    validator: (propsValue) => (propsValue ? true : false),
  },
  password: {
    type: String,
    required: true,
    validator: (propsValue) => (propsValue.length >= 6 ? true : false),
  },
});
</script>

<template>
  <div>
    <h1>hello from custom Validation prop Page</h1>
    <h1>{{ name }}</h1>
    <h1>{{ age }}</h1>
    <h1>{{ password }}</h1>
  </div>
</template>
