<template>
  <div>
    <div class="flex flex-wrap justify-center gap-10 text-center align-middle">
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
  </div>
</template>
