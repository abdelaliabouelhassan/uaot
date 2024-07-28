<template>
  <div class="w-full">
    <div
      class="w-full grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4 pt-4 lg:pb-12"
    >
      <nuxt-link to="/details" v-for="(item, index, key) in images" :key="key">
        <ImageCard
          :images="item.images"
          :count="item.count"
          :liked="item.liked"
          :type="item.type"
          :title="item.title"
          :name="item.name"
        />
      </nuxt-link>
    </div>
    <div class="w-full flex justify-end">
      <Pagination />
    </div>
  </div>
</template>

<script setup>
import Pagination from "@/components/UI/Pagination.vue";
import ImageCard from "@/components/UI/ImageCard.vue";
const props = defineProps(["images"]);
</script>
