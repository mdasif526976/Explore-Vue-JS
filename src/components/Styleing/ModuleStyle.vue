<template>
  <h1 v-bind:class="$style['m-class']">
    Styling with module and kabba case and $ syntex
  </h1>
  <h1 :class="$style['anotherclass']">Styling with CamelCase</h1>
  <h1 :class="bg.textStyle">Another module style system</h1>
</template>

<style module>
/* kabba case */
.m-class {
  background: purple;
  color: white;
}
/* Camel Case */
.anotherclass {
  background: seagreen;
  color: white;
}
</style>

// also another
<style module="bg">
.textStyle {
  background: cyan;
  color: white;
}
</style>
