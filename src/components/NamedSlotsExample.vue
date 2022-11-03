<template>
  <!-- Sometimes we should relegate styling to Vue's style block -->
  <!-- In this case, it's good to _scope_, and require lang="postcss"-->
  <div class="my-16 flex flex-wrap justify-center gap-10">
    <div class="flex max-w-fit">
      <slot name="left"></slot>
    </div>
    <div class="flex max-w-fit transition duration-500">
      <slot name="middle"></slot>
    </div>
    <div class="flex max-w-fit">
      <slot name="right"></slot>
    </div>
  </div>
</template>
