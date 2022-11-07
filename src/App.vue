<!-----------------------------------------------------------------------------
▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒
▒                                                                             ▒
▒  A Vite + Vue + Tailwind starter / learner project                          ▒
▒                                                                             ▒
▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒
------------------------------------------------------------------------------>
<script setup lang="ts">
import Example from "@/components/BaseExampleContainer.vue";
import Reactive from "@/components/examples/ReactiveComponentBasic.vue";
import Computed from "@/components/examples/ComputedProperties.vue";
import StyleBindings from "@/components/examples/StyleBindings.vue";
</script>

<template>
  <main class="my-24 mx-auto flex max-w-screen-md flex-col space-y-12">
    <Example title="Basic Reactivity">
      <Reactive />
    </Example>
    <Example title="Computed Properties">
      <Computed />
    </Example>
    <Example title="Class and Style Bindings">
      <StyleBindings />
    </Example>
  </main>
</template>
