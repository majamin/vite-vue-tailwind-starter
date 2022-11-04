<!----------------------------------------------------------------------------

  ~ Basic reactivity example ~

    * Component import
    * Props
    * Reactive values (via `ref`)
    * v-on handlers (using abrv. @)

----------------------------------------------------------------------------->

<template>
  <div
    class="my-8 flex flex-col justify-evenly bg-zinc-100 p-10 text-center align-middle shadow-md shadow-slate-400"
  >
    <div class="mt-4 mb-8 text-4xl font-black">{{ msg }}</div>
    <div class="mx-auto flex w-72 flex-row items-center justify-center">
      <!-- click-handler listens and passes the value emitted to addCount-->
      <div class="w-32">
        <BaseButton @click-handler="addCount">Add</BaseButton>
      </div>
      <!-- note: click-handler is defined in the component -->
      <div class="w-32 text-2xl">{{ count }}</div>
      <div class="w-32">
        <BaseButton @click-handler="resetCount">Reset</BaseButton>
      </div>
    </div>
    <p class="mt-6">
      <code class="text-xs">@/components/ReactiveComponentBasic.vue</code>
    </p>
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";
import BaseButton from "@/components/BaseButton.vue";

// This is a good way of defining props.
// Optionally, the constructor accepts an interface:
// defineProps<CustomInterface>();
defineProps<{ msg: string }>();

const count = ref(0);

// These functions are quite simple! Consider:
// 1. Using computed properties if you have complex logic and reactive data
// 2. Composables for reusable components
// https://vuejs.org/guide/reusability/composables.html
function addCount(clicked: boolean) {
  clicked ? (count.value++) : null;
}
function resetCount(clicked: boolean) {
  clicked ? (count.value = 0) : null;
}
</script>
