<template>
  <div class="w-full space-y-4 pt-10">
    <h3 class="font-assistant font-extrabold text-[#D68637] text-3xl">
      ABOUT ME
    </h3>

    <p class="font-assistant text-[#FFDDBB] text-base" v-html="about"></p>
  </div>
</template>

<script setup>
const props = defineProps(["about"]);
</script>
