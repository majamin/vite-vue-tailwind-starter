<script setup lang="ts">
const { customStyle } = defineProps<{ customStyle: string }>();
</script>
<template>
  <button type="button" :class="customStyle ? customStyle : 'bg-slate-500 text-slate-100' " class="min-w-[100px] text-white">
    <!-- Unnamed, default slot with default-->
    <slot>Submit</slot>
  </button>
</template>
