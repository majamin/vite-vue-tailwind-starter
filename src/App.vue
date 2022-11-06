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
import NamedSlots from "@/components/examples/NamedSlotsExample.vue";
</script>

<template>
  <main class="my-24 mx-auto flex max-w-screen-md flex-col space-y-12">
    <Example title="Basic Reactivity">
      <Reactive />
    </Example>
    <Example title="Computed Properties">
      <Computed name="there" />
    </Example>
    <Example title="Named Slots">
      <NamedSlots>
        <!-- note that the templates are out of order, but rendered correctly -->
        <template v-slot:middle> Middle </template>
        <template v-slot:left> Left </template>
        <template v-slot:right> Right </template>
      </NamedSlots>
    </Example>
  </main>
</template>
