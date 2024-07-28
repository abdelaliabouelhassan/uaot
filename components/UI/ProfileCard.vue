<template>
  <div class="flex items-center gap-4">
    <nuxt-link
      to="/profile"
      class="w-[160px] h-[160px] border border-[#FFDDBB]"
    >
      <img
        src="/images/Profilepicture_example.png"
        class="w-full h-full object-cover"
        alt=""
      />
    </nuxt-link>
    <div class="flex flex-col items-start space-y-3">
      <h4 class="text-[#D68637] font-assistant font-extrabold text-3xl">
        {{ name }}
      </h4>
      <span class="text-[#FFDDBB] font-assistant font-normal text-lg"
        >IGN: {{ ign }}</span
      >

      <div class="flex items-center gap-4">
        <div class="flex items-center gap-2">
          <img
            src="/images/icons/active-heart.svg"
            class="w-[19px] h-[19px] object-cover"
            alt=""
          />
          <span class="text-[#FFDDBB] font-assistant font-normal text-lg">{{
            likes
          }}</span>
        </div>
        <div class="flex items-center gap-2">
          <img
            src="/images/icons/shirt.png"
            class="w-[19px] h-[19px] object-cover"
            alt=""
          />
          <span class="text-[#FFDDBB] font-assistant font-normal text-lg">{{
            images
          }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const props = defineProps(["ign", "name", "likes", "images"]);
</script>
