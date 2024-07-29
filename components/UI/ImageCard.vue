<template>
  <div
    @mouseover="ChangeImages"
    @mouseout="CleanTl"
    class="w-full h-[641px] bg-gray-400 relative cursor-pointer group/card overflow-hidden"
  >
    <div class="absolute top-2 left-2">
      <img :src="type" class="w-7 h-7 object-cover" alt="" />
    </div>

    <img
      v-for="(image, index) in images"
      :key="index"
      :src="image"
      :class="{ show: index === currentIndex, hide: index !== currentIndex }"
      class="w-full h-full object-cover image duration-300"
    />

    <div
      class="absolute -bottom-40 left-0 w-full group-hover/card:bottom-10 duration-300"
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
const props = defineProps([
  "images",
  "type",
  "liked",
  "count",
  "title",
  "name",
]);

const liked = ref(props.liked);
const count = ref(props.count);
const currentIndex = ref(0);
const totalImages = ref(0);
const tl = ref(null);

const like = () => {
  liked.value = !liked.value;
  if (liked.value) {
    count.value++;
  } else {
    count.value--;
  }
};

const ChangeImages = () => {
  tl.value = setInterval(() => {
    if (currentIndex.value < totalImages.value - 1) {
      currentIndex.value++;
    } else {
      currentIndex.value = 0;
    }
  }, 2000);
};

const CleanTl = () => {
  clearInterval(tl.value);
  tl.value = null;
};

onMounted(() => {
  totalImages.value = props.images.length;
});
</script>

<style scoped>
.textShdow {
  text-shadow: 1px 1px 1px #00000059;
}

.image {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  transition: opacity 0.5s ease-in-out, transform 0.5s ease-in-out;
  opacity: 0;
  transform: scale(1);
}

.image.show {
  opacity: 1;
  transform: scale(1.1); /* Adjust the scale value for zoom effect */
}

.image.hide {
  opacity: 0;
  transform: scale(1);
}
</style>
