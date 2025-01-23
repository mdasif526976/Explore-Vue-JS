<script setup></script>
<template>
  <div>
    <h1>Component Event from child</h1>
    <button @click="$emit('increment')">Emit Event</button>
  </div>
</template>
