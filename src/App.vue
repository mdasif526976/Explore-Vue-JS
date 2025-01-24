<script setup>
import { provide, ref } from "vue";
import ComponentEvent from "./components/Component Events/ComponentEvent.vue";
import Computed from "./components/Computed Properties/Computed.vue";
import Conditional from "./components/Conditional Renderring/Conditional.vue";
import Counter from "./components/Events/Counter.vue";
import Input from "./components/Events/Input.vue";
import Itaration from "./components/ItarationComponent/Itaration.vue";
import WithApi from "./components/ItarationComponent/WithApi.vue";
import Reactive from "./components/My Reactive Component/Reactive.vue";
import View from "./components/Props/View.vue";
import SlotComponent from "./components/Slots/SlotComponent.vue";
import SlotsView from "./components/Slots/SlotsView.vue";
import CombineStyle from "./components/Styleing/CombineStyle.vue";
import GlobalStyle from "./components/Styleing/GlobalStyle.vue";
import LocalStyle from "./components/Styleing/LocalStyle.vue";
import ModuleStyle from "./components/Styleing/ModuleStyle.vue";
import Form from "./components/Use v-model/Form.vue";
import School from "./components/Provide & Inject/School.vue";
import LifecycleHooks from "./components/LifeCycle Hooks/LifecycleHooks.vue";
import Watch from "./components/Watchers/Watch.vue";
const title = ref("My Vue js Website");
document.title = title.value;
const user = ref({ name: "Ali Mahmud", age: 20, class: "100" });
provide("student", user);
const show = ref(true);
</script>
<template>
  <div>
    <Watch />
  </div>
  <!-- <LifecycleHooks v-if="show" /> -->
  <!-- <button @click="show = !show">hide</button> -->
</template>
