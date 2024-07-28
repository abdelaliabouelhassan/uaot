<template>
  <div
    class="text-lg text-[#FFDDBB] font-assistant bg-[#272727] px-4 py-1"
    :style="{ 'background-color': bg }"
  >
    {{ text }}
  </div>
</template>

<script setup>
const props = defineProps(["text", "bg"]);
</script>
