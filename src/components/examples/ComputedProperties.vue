<!-----------------------------------------------------------------------------
▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒
▒                                                                             ▒
▒   ~ Computed properties ~                                                   ▒
▒   Computed properties are cached and only update when their                 ▒
▒   dependencies change.                                                      ▒
▒   https://vuejs.org/guide/essentials/reactivity-fundamentals.html           ▒
▒                                                                             ▒
▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒
------------------------------------------------------------------------------>
<script setup lang="ts">
import { computed } from "vue";

// Option 1: Pure type annotation
const { name } = defineProps<{ name: string }>();

// Option 2: Object declaration
// const { title } = defineProps({ title: String });

// Or, use a custom interface:
// const { title } = defineProps<CustomInterface>();

// computed properties are cached and only update
// when their dependencies change
const greeting = computed(() => {
  return "Hello, " + name + "!";
});
</script>

<template>
  <div>
    <div>{{ greeting }}</div>
  </div>
</template>
