<template>
  <div class="flex items-center gap-3 text-[#FFDDBB] font-assistant">
    <span class="text-xl">Page</span>
    <button
      @click="changePage(page)"
      v-for="(page, index, key) in pages"
      :key="key"
      class="hover:font-bold"
      :class="{
        'bg-[#41081C] w-[12px] text-[#D68637] font-bold': activePage == page,
      }"
    >
      {{ page }}
    </button>
  </div>
</template>

<script setup>
const pages = ref([1, 2, 3, 4, 5, 6, 7]);

const activePage = ref(1);

const changePage = (page) => {
  activePage.value = page;
};
</script>
