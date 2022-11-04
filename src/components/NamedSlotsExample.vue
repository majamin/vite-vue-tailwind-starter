<template>
  <!-- Sometimes we should relegate styling to Vue's style block -->
  <!-- In this case, it's good to _scope_, and require lang="postcss"-->
  <div class="my-8 bg-zinc-100 p-10 shadow-md shadow-slate-400">
    <div class="mt-4 mb-8 text-4xl font-black">{{ msg }}</div>
    <div class="flex flex-wrap justify-center gap-10 text-center align-middle">
      <div class="flex max-w-fit">
        <slot name="left"></slot>
      </div>
      <div class="flex max-w-fit transition duration-500">
        <slot name="middle"></slot>
      </div>
      <div class="flex max-w-fit">
        <slot name="right"></slot>
      </div>
    </div>
    <p class="mt-6">
      <code class="text-xs">@/components/NamedSlotsExample.vue</code>
    </p>
  </div>
</template>

<script setup lang="ts">
defineProps<{ msg: string }>();
</script>
