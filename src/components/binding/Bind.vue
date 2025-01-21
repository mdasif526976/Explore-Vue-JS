<script setup>
import image from "../../assets/asif.jpg";
// static binding
const alt = "Md Asif";
const height = 400;
const weight = 300;
// two way you can bind  {:v-bind}--old way or colon(:)--new way

//dynamic data binding
const imageInfo = { src: image, alt: "Md Asif", height: 400, width: 300 };
</script>
<template>
  <img :src="image" :height="height" :width="weight" :v-bind="alt" />
  dynamic way
  <img src="" alt="" />
  <img :="imageInfo" />
</template>
