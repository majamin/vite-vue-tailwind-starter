<!-----------------------------------------------------------------------------
▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒
▒                                                                             ▒
▒                                                                             ▒
▒                                                                             ▒
▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒
------------------------------------------------------------------------------>

<script setup lang="ts">
import CTASimpleCenter from "@/components/full/CTASimpleCenter.vue";
import BaseButton from "@/components/base/BaseButton.vue";
</script>
<template>
  <div class="flex flex-col md:flex-row overflow-hidden">
    <div class="flex items-center justify-center overflow-hidden md:w-4/5">
      <img
        class="object-cover w-full h-full"
        src="meeting.jpg"
        alt=""
      />
    </div>
    <div class="w-full md:w-4/5 bg-indigo-600 p-10 text-white">
      <div class="text-4xl font-extrabold">
        <slot name="title"
          >Boost your productivity.<br />Start using Awsme today.</slot
        >
      </div>
      <div class="mx-auto mt-4 max-w-xl text-slate-200">
        <slot name="text">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo, cum,
          quidem vitae eius hic animi nihil sequi nostrum exercitationem rem
          corporis nemo optio distinctio tempora quis blanditiis alias impedit
          cupiditate.
        </slot>
      </div>
      <BaseButton class="my-10" :customStyle="'bg-slate-100 text-indigo-800'"
        ><slot>Sign up for free</slot></BaseButton
      >
    </div>
  </div>
</template>
