<script setup lang="ts">

const emit = defineEmits<{
  (event: 'count-handler', clicked: boolean): void;
}>()
</script>

<template>
  <button
    @click="emit('count-handler', true)"
    type="button"
    class="max-w-fit bg-sky-600 text-white"
  >
    <slot>Submit</slot>
  </button>
</template>
