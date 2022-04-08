<template>
  <div
    class="bg-black h-screen flex-col items-center flex justify-center align-top text-gray-400 w-screen text-center"
  >
    <div class="text-left flex flex-col gap-4">
      <div class="text-5xl text-slate-300 font-semibold">Krish</div>
      <div class="text-3xl">i built shit soemtimes</div>
      <div class="w-96 text-xl">
        I'm a software engineer and artist based in Toronto. I have great
        interest in full-stack development, artificial intelligence,
        human-computer interactions, and everything in between.
      </div>
    </div>
    <ArrowCircleDownIcon class="h-24"></ArrowCircleDownIcon>
  </div>
</template>

<script lang="ts">
import { ArrowCircleDownIcon } from "@heroicons/vue/solid";

export default {
  components: { ArrowCircleDownIcon },
};
</script>
