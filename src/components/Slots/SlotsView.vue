<script setup>
import DefaultSlot from "./DefaultSlot.vue";
import FallbackContent from "./FallbackContent.vue";
import NameSlot from "./NameSlot.vue";
import SlotComponent from "./SlotComponent.vue";
</script>

<template>
  <div>
    <SlotComponent> hello world </SlotComponent>
    <hr />
    <FallbackContent></FallbackContent>
    <FallbackContent
      ><h1>
        FallbackSlots not work here cause i provide some content
      </h1></FallbackContent
    >

    <!-- name slots -->
    <!-- you can access name slots by {v-slot:} {#:} -->
    <hr />
    <NameSlot>
      <template v-slot:firstSlot>
        <h1>this content going to slot no 1</h1>
      </template>
      <hr />
      <template #secondSlot>
        <h1>this content going to slot no 2</h1>
      </template>
    </NameSlot>

    <hr />
    <DefaultSlot>
      <template #default>
        <h1>hello from default slot</h1>
      </template>
    </DefaultSlot>
  </div>
</template>
