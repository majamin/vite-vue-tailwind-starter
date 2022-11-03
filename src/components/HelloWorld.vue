<script setup lang="ts">
import { ref } from "vue";
import BaseButton from "@/components/BaseButton.vue";

// This is a good way of defining props.
// Optionally, the constructor accepts an interface:
// defineProps<CustomInterface>();
defineProps<{ msg: string }>();

const count = ref(0);

// These functions are quite simple!
// With greater complexity, consider using the "composable" pattern
// https://vuejs.org/guide/reusability/composables.html
function addCount(clicked: boolean) {
  clicked ? (count.value += 1) : null;
}
function resetCount(clicked: boolean) {
  clicked ? (count.value = 0) : null;
}
</script>

<template>
  <div
    class="my-4 flex h-36 flex-col justify-evenly bg-zinc-100 text-center align-middle"
  >
    <div class="mx-auto flex w-72 flex-row items-center justify-evenly">
      <!-- click-handler listens and passes the value emitted to addCount-->
      <BaseButton @click-handler="addCount">Add</BaseButton>
      <!-- note: click-handler is defined in the component -->
      <div class="text-2xl">{{ count }}</div>
      <BaseButton @click-handler="resetCount">Reset</BaseButton>
    </div>
    <p>
      Edit
      <code>components/BasicProps.vue</code> to test HMR
    </p>
  </div>
</template>
