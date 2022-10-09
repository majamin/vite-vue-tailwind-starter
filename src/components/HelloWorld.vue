<script setup lang="ts">
import { ref } from "vue";

defineProps<{ msg: string }>();

const count = ref(0);
</script>

<template>
  <h1 class="my-4 text-4xl text-sky-800">{{ msg }}</h1>

  <div
    class="my-4 flex h-36 flex-col justify-evenly bg-zinc-100 text-center align-middle"
  >
    <button
      class="mx-auto max-w-fit bg-sky-600 text-white"
      type="button"
      @click="count++"
    >
      count is {{ count }}
    </button>
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
