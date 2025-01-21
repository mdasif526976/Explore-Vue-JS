<script setup>
import { ref } from "vue";
import DynamicProps from "./DynamicProps.vue";
import StaticProps from "./StaticProps.vue";
import Validation from "./Validation.vue";
import CustomValiddationProp from "./CustomValiddationProp.vue";
const fName = ref("Md");
const lName = ref("Asif");
let anotherAge = ref(40);
</script>

<template>
  <h1>Define a component that accepts props and displays them.</h1>
  <!-- 
  <hr />
  <StaticProps user="Md Asif" />
  <hr />
  <DynamicProps v-bind:firstName="fName" :lastName="lName" />
  <hr />
  <Validation :firstName="fName" age="20" /> -->
  <CustomValiddationProp name="Md Asif" :age="30" password="d0fd122d" />
</template>
