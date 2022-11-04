<template>
  <div>
    <div>{{ greeting(name).value }}</div>
  </div>
</template>

<script setup lang="ts">
import { computed } from "vue";

const { name } = defineProps<{ name: string }>();

const greeting = (str: string) =>
  computed(() => {
    return "Hello, " + str + "!";
  });
</script>
