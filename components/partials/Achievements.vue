<template>
  <div class="flex flex-col items-start gap-4">
    <h2 class="font-assistant font-extrabold text-[#D68637] text-3xl">
      ACHIEVEMENTS
    </h2>
    <div class="flex items-start flex-wrap gap-3">
      <div
        class="w-[80px] h-[80px] rounded-full bg-[#FFDDBB]"
        v-for="n in 4"
        :key="n"
      ></div>
      <div
        class="w-[80px] h-[80px] rounded-full border-2 border-[#D68637] flex"
      >
        <span class="m-auto text-[#FFDDBB] text-4xl font-assistant">+ 5</span>
      </div>
    </div>
  </div>
</template>
