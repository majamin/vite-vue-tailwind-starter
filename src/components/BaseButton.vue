<script setup lang="ts">
// type-safe emit
const emit = defineEmits<{
  (event: "click-handler", clicked: boolean): void;
}>();
</script>

<template>
  <button
    @click="emit('click-handler', true)"
    type="button"
    class="bg-sky-600 text-white min-w-[100px]"
  >
    <!-- Unnamed, default slot with default-->
    <slot>Submit</slot>
  </button>
</template>
