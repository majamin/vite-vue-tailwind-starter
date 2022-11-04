<!----------------------------------------------------------------------------

  A starter template / learning project

  Vite + Vue + Tailwind (w. Typescript)
    Tailwind for styling
      Composition API using script setup

----------------------------------------------------------------------------->
<script setup lang="ts">
import ReactiveComponentBasic from "@/components/examples/ReactiveComponentBasic.vue";
import NamedSlotsExample from "@/components/examples/NamedSlotsExample.vue";
import ComputedProperties from "@/components/examples/ComputedProperties.vue";
import Example from "@/components/BaseExampleContainer.vue";
</script>

<template>
  <main class="my-24 mx-auto flex max-w-screen-md flex-col space-y-12">
    <!--------------------------
      Basic reactivity and props
    --------------------------->
    <Example title="Basic Reactivity">
      <ReactiveComponentBasic />
    </Example>
    <!-------------------
      Computed properties
    -------------------->
    <Example title="Computed Properties">
      <ComputedProperties name="Bozo"></ComputedProperties>
    </Example>
    <!-------------
      Named slots
    -------------->
    <Example title="Named Slots">
      <NamedSlotsExample>
        <template v-slot:left>
          <div class="h-36 w-36 bg-amber-500"></div>
        </template>
        <template v-slot:middle>
          <div class="h-36 w-36 bg-cyan-500"></div>
        </template>
        <template v-slot:right>
          <div class="h-36 w-36 bg-fuchsia-500"></div>
        </template>
      </NamedSlotsExample>
    </Example>
  </main>
</template>
