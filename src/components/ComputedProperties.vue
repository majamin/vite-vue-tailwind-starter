<template>
  <div class="my-8 bg-zinc-100 p-10 shadow-md shadow-slate-400">
    <div class="mt-4 mb-8 text-4xl font-black">Computed Properties</div>
    <div>{{ greeting }}</div>
  </div>
</template>

<script setup lang="ts">
import { computed } from "vue";

const { name } = defineProps<{ name: string }>();

const greeting = computed(() => {
  return "Hello, " + name + "!";
});
</script>
