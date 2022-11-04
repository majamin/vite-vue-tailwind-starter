<!----------------------------------------------------------------------------

  A starter template / learning project

  Vite + Vue + Tailwind (w. Typescript)
    Tailwind for styling
      Composition API using script setup

----------------------------------------------------------------------------->
<script setup lang="ts">
import ReactiveComponentBasic from "@/components/ReactiveComponentBasic.vue";
import NamedSlotsExample from "@/components/NamedSlotsExample.vue";
import ComputedProperties from "@/components/ComputedProperties.vue";
</script>

<template>
  <main class="my-24 mx-auto max-w-screen-md">
    <!--------------------------
      Basic reactivity and props
    --------------------------->
    <ReactiveComponentBasic msg="Basic Reactivity" />
    <!-------------
      Named slots
    -------------->
    <NamedSlotsExample msg="Named Slots">
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
    <!-------------------
      Computed properties
    -------------------->
    <ComputedProperties name="Marian" />
  </main>
</template>
