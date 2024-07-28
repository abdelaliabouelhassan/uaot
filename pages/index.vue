<template>
  <section class="bg-[#272727] pt-6 pb-8 lg:pb-16">
    <div class="w-full max-w-[1437px] mx-auto px-4 space-y-4">
      <Filter />
      <div class="w-full border-[0.5px] border-[#83838363]"></div>

      <GridImages :images="Images" />
    </div>
  </section>
</template>

<script setup>
import ImageCard from "@/components/UI/ImageCard.vue";
import GridImages from "@/components/UI/GridImages.vue";
import Filter from "@/components/UI/Filter.vue";
const Images = ref([
  {
    images: ["/images/Placeholder4.jpg", "/images/Placeholder3.jpg"],
    liked: true,
    count: 17,
    type: "/images/types/type1.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    images: ["/images/Placeholder3.jpg", "/images/Placeholder2.jpg"],
    liked: false,
    count: 6,
    type: "/images/types/type2.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    images: ["/images/Placeholder1.png", "/images/Placeholder2.jpg"],
    liked: false,
    count: 27,
    type: "/images/types/type3.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    images: [
      "/images/Placeholder2.jpg",
      "/images/Placeholder6.jpg",
      "/images/Placeholder7.jpg",
    ],
    liked: true,
    count: 12,
    type: "/images/types/type4.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    images: [
      "/images/Placeholder1.jpg",
      "/images/Placeholder6.jpg",
      "/images/Placeholder7.jpg",
    ],
    liked: false,
    count: 17,
    type: "/images/types/type5.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    images: [
      "/images/Placeholder5.jpg",
      "/images/Placeholder6.jpg",
      "/images/Placeholder7.jpg",
    ],
    liked: true,
    count: 40,
    type: "/images/types/type6.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    images: ["/images/Placeholder6.jpg", "/images/Placeholder7.jpg"],
    liked: false,
    count: 5,
    type: "/images/types/type7.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    images: ["/images/Placeholder7.jpg"],
    liked: false,
    count: 15,
    type: "/images/types/type8.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    images: [
      "/images/Placeholder1.png",
      "/images/Placeholder7.jpg",
      "/images/Placeholder2.jpg",
      "/images/Placeholder6.jpg",
      "/images/Placeholder7.jpg",
    ],
    liked: false,
    count: 27,
    type: "/images/types/type3.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    images: ["/images/Placeholder2.jpg"],
    liked: true,
    count: 12,
    type: "/images/types/type4.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    images: ["/images/Placeholder1.jpg"],
    liked: false,
    count: 17,
    type: "/images/types/type5.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    images: ["/images/Placeholder5.jpg"],
    liked: true,
    count: 40,
    type: "/images/types/type6.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
]);
</script>
