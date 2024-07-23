<template>
  <div
    class="w-full h-[641px] bg-gray-400 relative cursor-pointer group/card overflow-hidden"
  >
    <div class="absolute top-2 left-2">
      <img :src="type" class="w-7 h-7 object-cover" alt="" />
    </div>
    <img :src="image" class="w-full h-full object-cover" alt="" />

    <div
      class="absolute -bottom-40 left-0 w-full group-hover/card:bottom-10 duration-100"
    >
      <div class="w-full p-4 space-y-2">
        <h5 class="font-bold font-assistant text-[#FFDDBB] text-xl">
          {{ title }}
        </h5>
        <div class="w-full border-2 border-[#D68637] max-w-[235px]"></div>
        <span class="text-sm text-[#FFDDBB]">{{ name }}</span>
      </div>
    </div>

    <div class="flex items-center absolute bottom-4 right-3 gap-2 space-y-1">
      <span
        class="font-assistant text-[#FFDDBB] font-bold text-2xl textShdow"
        >{{ count }}</span
      >
      <button class="group" @click="like">
        <img
          src="/images/icons/heart.svg"
          class="w-7 h-7 object-cover"
          alt=""
        />
        <img
          src="/images/icons/active-heart.svg"
          class="w-[26px] h-[25px] object-cover absolute bottom-1 right-[1px] group-hover:block"
          :class="{ hidden: !liked }"
          alt=""
        />
      </button>
    </div>
  </div>
</template>

<script setup>
const props = defineProps(["image", "type", "liked", "count", "title", "name"]);

const liked = ref(props.liked);
const count = ref(props.count);

const like = () => {
  liked.value = !liked.value;
  if (liked.value) {
    count.value++;
  } else {
    count.value--;
  }
};
</script>

<style scoped>
.textShdow {
  text-shadow: 1px 1px 1px #00000059;
}
</style>
