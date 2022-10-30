<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import HelloWorld from "@/components/HelloWorld.vue";
</script>

<template>
  <!-- Tailwindcss styling -->
  <main class="my-24 mx-auto max-w-screen-md">
    <div class="my-16 flex justify-center">
      <div class="mx-10 w-1/3">
        <a href="https://vitejs.dev" target="_blank">
          <img
            src="vite.svg"
            class="mx-auto w-32 transition-all duration-200 ease-in-out will-change-auto hover:shadow-gray-900 hover:drop-shadow-xl"
            alt="Vite logo"
          />
          <h1 class="my-4 font-serif text-5xl text-violet-500">Vite</h1>
        </a>
      </div>
      <div class="mx-10 w-1/3">
        <a href="https://vuejs.org/" target="_blank">
          <img
            src="@/assets/vue.svg"
            class="mx-auto w-32 transition-all duration-200 ease-in-out will-change-auto hover:shadow-gray-900 hover:drop-shadow-xl"
            alt="Vite logo"
          />
          <h1 class="my-4 font-serif text-5xl text-[#41b883]">Vue</h1>
        </a>
      </div>
      <div class="mx-10 w-1/3">
        <a href="https://vuejs.org/" target="_blank">
          <img
            src="@/assets/tailwind.svg"
            class="mx-auto w-32 transition-all duration-200 ease-in-out will-change-auto hover:shadow-gray-900 hover:drop-shadow-xl"
            alt="Vite logo"
          />
          <h1 class="my-4 font-serif text-5xl text-[#00b7d6]">Tailwind</h1>
        </a>
      </div>
    </div>
    <!-- HelloWorld is a component receiving props -->
    <HelloWorld msg="Vite + Vue" />
  </main>
</template>
