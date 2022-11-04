<template>
  <div>
    <div class="text-3xl font-black text-zinc-600">{{ title }}</div>
    <div
      class="mt-2 flex flex-col justify-evenly bg-zinc-100 p-10 text-center align-middle shadow-md shadow-slate-400"
    >
      <slot></slot>
    </div>
  </div>
</template>

<script setup lang="ts">
// This is a good way of defining props.
// Optionally, the constructor accepts an interface:
// defineProps<CustomInterface>();
const { title } = defineProps<{ title: string }>();
</script>
