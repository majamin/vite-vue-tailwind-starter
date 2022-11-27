<!-----------------------------------------------------------------------------
▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒
▒                                                                             ▒
▒  A Vite + Vue + Tailwind starter / learner project                          ▒
▒                                                                             ▒
▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒
------------------------------------------------------------------------------>
<script setup lang="ts">
import Example from "@/components/single/ExampleContainer.vue";
import Reactive from "@/components/single/ReactiveComponentBasic.vue";
import Computed from "@/components/single/ComputedProperties.vue";
import StyleBindings from "@/components/single/StyleBindings.vue";
import Conditional from "@/components/single/Conditional.vue";

import Feature2x2Grid from "@/components/full/Feature2x2Grid.vue";
import CTASimpleCenter from "@/components/full/CTASimpleCenter.vue";
import CTASplitImage from "@/components/full/CTASplitImage.vue";
import PageSectionFAQ from "@/components/full/PageSectionFAQ.vue";
</script>

<template>
  <main class="my-24 flex flex-col space-y-12">
    <Example class="container mx-auto" title="Basic Reactivity">
      <Reactive />
    </Example>
    <Example class="container mx-auto" title="Computed Properties">
      <Computed />
    </Example>
    <Example class="container mx-auto" title="Class and Style Bindings">
      <StyleBindings />
    </Example>
    <Example class="container mx-auto" title="Conditional Rendering">
      <Conditional />
    </Example>
    <Feature2x2Grid class="bg-sky-200">
      <template v-slot:title>Feature</template>
      <template v-slot:tagline></template>
      <template v-slot:tagline-more>A very clever quote</template>
    </Feature2x2Grid>
    <CTASimpleCenter class="container mx-auto" />
    <!-- <CTASplitImage class="container mx-auto sm:rounded-md" /> -->
    <CTASplitImage />
    <PageSectionFAQ />
  </main>
</template>
