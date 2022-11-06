<!-----------------------------------------------------------------------------
▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒
▒                                                                             ▒
▒   ~ Basic reactivity example ~                                              ▒
▒   `reactive` elements are js proxies and behave like objects.               ▒
▒   Vue can track property access and mutations on reactive elements.         ▒
▒   https://vuejs.org/guide/essentials/reactivity-fundamentals.html           ▒
▒                                                                             ▒
▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒
------------------------------------------------------------------------------>
<script setup lang="ts">
import BaseButton from "@/components/BaseButton.vue";
import { reactive } from "vue";

//------------ No typing ------------------------------------------------------
const state = reactive({ count: 0 });

/*------------ With typing ----------------------------------------------------
interface MyState {
  count: number;
}
const state: MyState = reactive({ count: 0 });
-----------------------------------------------------------------------------*/

function increment() {
  state.count++;
}
function reset() {
  state.count = 0;
}
</script>

<template>
  <div>
    <div class="mx-auto flex w-72 flex-row items-center justify-center">
      <div class="w-32">
        <BaseButton @click="increment">+1</BaseButton>
      </div>
      <div class="w-32 text-2xl">{{ state.count }}</div>
      <div class="w-32">
        <BaseButton @click="reset">Reset</BaseButton>
      </div>
    </div>
  </div>
</template>
