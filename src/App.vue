<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import HelloWorld from "@/components/HelloWorld.vue";
</script>

<template>
  <main class="mx-auto max-w-screen-md">
    <div>
      <a href="https://vitejs.dev" target="_blank">
        <img
          src="vite.svg"
          class="mx-auto my-4 h-32 transition-all duration-200 ease-in-out will-change-auto hover:shadow-gray-900 hover:drop-shadow-xl"
          alt="Vite logo"
        />
      </a>
      <a href="https://vuejs.org/" target="_blank">
        <img
          src="@/assets/vue.svg"
          class="mx-auto my-4 h-32 transition-all duration-200 ease-in-out will-change-auto hover:shadow-gray-900 hover:drop-shadow-xl"
          alt="Vue logo"
        />
      </a>
    </div>
    <HelloWorld msg="Vite + Vue" />
  </main>
</template>
