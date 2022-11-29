<!-----------------------------------------------------------------------------
▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒
▒                                                                             ▒
▒  A Vite + Vue + Tailwind starter / learner project                          ▒
▒                                                                             ▒
▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒
------------------------------------------------------------------------------>
<script setup lang="ts">
import Example from "@/components/VueBasics/ExampleContainer.vue";
import Reactive from "@/components/VueBasics/ReactiveComponentBasic.vue";
import Computed from "@/components/VueBasics/ComputedProperties.vue";
import StyleBindings from "@/components/VueBasics/StyleBindings.vue";
import Conditional from "@/components/VueBasics/Conditional.vue";

import Feature2x2Grid from "@/components/Sections/PageFeat2x2GridCentered.vue";
import CTASimpleCenter from "@/components/Sections/CTASimpleCenter.vue";
import CTASplitImage from "@/components/Sections/CTASplitImage.vue";
import PageSectionFAQ from "@/components/Faq/PageSectionFAQ.vue";
import TableTemplate from "@/components/Lists/TableTemplate.vue";
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
    <PageSectionFAQ class="container mx-auto" />
    <TableTemplate class="container mx-auto" />
  </main>
</template>
