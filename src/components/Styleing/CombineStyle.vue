<template>
  <h1 class="text-h1">im from combineStyle</h1>
  <h1 class="text-l1">im from combineStyle local Style</h1>
</template>

// this for globalStyle
<style>
.text-h1 {
  background: green;
  color: white;
}
</style>

// this for localStyle
<style scoped>
.text-l1 {
  background: yellow;
  color: white;
}
</style>
