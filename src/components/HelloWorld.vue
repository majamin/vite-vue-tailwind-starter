<script setup lang="ts">
import { ref } from "vue";
import BaseButton from "@/components/BaseButton.vue";

// This is the most succinct way of defining props.
// The constructor accepts can accept an interface:
// defineProps<CustomInterface>();
defineProps<{ msg: string }>();

const count = ref(0);

// These functions are simple so we don't import them
function addCount(clicked: boolean) {
  clicked ? count.value += 1 : null
}

function resetCount(clicked: boolean) {
  clicked ? count.value = 0 : null
}

</script>

<template>
  <h1 class="my-4 text-4xl text-sky-800">{{ msg }}</h1>

  <div
    class="my-4 flex h-36 flex-col justify-evenly bg-zinc-100 text-center align-middle"
  >
    <div class="mx-auto flex w-52 items-center justify-between">
      <!-- Component that listens and calls a function -->
      <BaseButton @click-handler="addCount">Add</BaseButton>
      <div class="text-2xl">{{ count }}</div>
      <BaseButton @click-handler="resetCount">Reset</BaseButton>
    </div>
    <p>
      Edit
      <code>components/HelloWorld.vue</code> to test HMR
    </p>
  </div>

  <p>
    Check out
    <a href="https://vuejs.org/guide/quick-start.html#local" target="_blank"
      >create-vue</a
    >, the official Vue + Vite starter
  </p>
</template>
