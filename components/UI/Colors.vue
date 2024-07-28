<template>
  <div
    class="grid gap-1 max-w-[80px] h-[83px] w-full"
    :class="{ 'grid-cols-2': count >= 3, 'grid-cols-1': count <= 2 }"
  >
    <button
      class="w-full h-[40px]"
      :class="{
        ' col-span-full': count === 3 && index === count - 1,
        ' h-[83px]': count === 1,
      }"
      :style="{ 'background-color': color }"
      v-for="(color, index, key) in colors"
      :key="key"
    ></button>
    {{ count }}
  </div>
</template>

<script setup>
const props = defineProps(["colors"]);
const count = ref(0);

onMounted(() => {
  count.value = props.colors.length;
});
</script>
