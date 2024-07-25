<template>
  <section class="bg-[#272727] pt-6 pb-8 lg:pb-16">
    <div class="w-full max-w-[1437px] mx-auto px-4 space-y-4">
      <form class="flex md:justify-end w-full pb-4">
        <div
          class="flex md:flex-row flex-col items-start gap-4 w-full md:w-fit"
        >
          <div class="flex flex-col items-start gap-1 w-full md:w-fit">
            <label
              for="orderby"
              class="text-[#D68637] font-bold font-assistant text-sm"
              >ORDER BY</label
            >
            <select
              name="orderby"
              id="orderby"
              class="text-[#FFDDBB] font-assistant text-sm bg-[#171717] py-3 px-2 outline-none w-full"
            >
              <option value="">NEWEST</option>
            </select>
          </div>
          <div class="flex flex-col items-start gap-1 w-full md:w-fit">
            <label
              for="race"
              class="text-[#D68637] font-bold font-assistant text-sm"
              >RACE</label
            >
            <select
              name="race"
              id="race"
              class="text-[#FFDDBB] font-assistant text-sm bg-[#171717] py-3 px-2 outline-none w-full"
            >
              <option value="">SYLVARI</option>
            </select>
          </div>
          <div class="flex flex-col items-start gap-1 w-full md:w-fit">
            <label
              for="race"
              class="text-[#D68637] font-bold font-assistant text-sm"
              >GENDER</label
            >
            <select
              name="gender"
              id="gender"
              class="text-[#FFDDBB] font-assistant text-sm bg-[#171717] py-3 px-2 outline-none w-full"
            >
              <option value="">FEMALE</option>
            </select>
          </div>
          <div class="flex flex-col items-start gap-1 w-full md:w-fit">
            <label
              for="weight"
              class="text-[#D68637] font-bold font-assistant text-sm"
              >WEIGHT</label
            >
            <select
              name="weight"
              id="weight"
              class="text-[#FFDDBB] font-assistant text-sm bg-[#171717] py-3 px-2 outline-none w-full"
            >
              <option value="">LIGHT</option>
            </select>
          </div>
          <div class="flex flex-col items-start gap-1 w-full md:w-fit">
            <label
              for="other"
              class="text-[#D68637] font-bold font-assistant text-sm"
              >OTHER FILTERS</label
            >
            <select
              name="other"
              id="other"
              class="text-[#FFDDBB] font-assistant text-sm bg-[#171717] py-3 px-2 outline-none w-full"
            >
              <option value="">PINK</option>
            </select>
          </div>
          <div class="flex flex-col items-start gap-1 w-full md:w-fit">
            <label
              for="search"
              class="text-[#D68637] font-bold font-assistant text-sm"
              >KEYWORD SEARCH</label
            >
            <div class="relative w-full md:w-fit">
              <div class="absolute left-2 top-3">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke-width="1.5"
                  stroke="currentColor"
                  class="size-[19px] text-[#3F3F3F]"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="m21 21-5.197-5.197m0 0A7.5 7.5 0 1 0 5.196 5.196a7.5 7.5 0 0 0 10.607 10.607Z"
                  />
                </svg>
              </div>
              <input
                type="text"
                class="bg-[#171717] py-3 outline-none placeholder-[#3F3F3F] text-[#FFDDBB] pl-8 text-sm pr-4 w-full md:w-fit"
                placeholder="KEYWORD OR USER"
              />
            </div>
          </div>
        </div>
      </form>

      <div class="w-full border-[0.5px] border-[#83838363]"></div>

      <div
        class="w-full grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4 pt-4 lg:pb-12"
      >
        <nuxt-link
          to="/details"
          v-for="(item, index, key) in Images"
          :key="key"
        >
          <ImageCard
            :image="item.image"
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
  </section>
</template>

<script setup>
import ImageCard from "@/components/UI/ImageCard.vue";
import Pagination from "@/components/UI/Pagination.vue";
const Images = ref([
  {
    image: "/images/Placeholder4.jpg",
    liked: true,
    count: 17,
    type: "/images/types/type1.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    image: "/images/Placeholder3.jpg",
    liked: false,
    count: 6,
    type: "/images/types/type2.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    image: "/images/Placeholder1.png",
    liked: false,
    count: 27,
    type: "/images/types/type3.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    image: "/images/Placeholder2.jpg",
    liked: true,
    count: 12,
    type: "/images/types/type4.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    image: "/images/Placeholder1.jpg",
    liked: false,
    count: 17,
    type: "/images/types/type5.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    image: "/images/Placeholder5.jpg",
    liked: true,
    count: 40,
    type: "/images/types/type6.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    image: "/images/Placeholder6.jpg",
    liked: false,
    count: 5,
    type: "/images/types/type7.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    image: "/images/Placeholder7.jpg",
    liked: false,
    count: 15,
    type: "/images/types/type8.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    image: "/images/Placeholder1.png",
    liked: false,
    count: 27,
    type: "/images/types/type3.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    image: "/images/Placeholder2.jpg",
    liked: true,
    count: 12,
    type: "/images/types/type4.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    image: "/images/Placeholder1.jpg",
    liked: false,
    count: 17,
    type: "/images/types/type5.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
  {
    image: "/images/Placeholder5.jpg",
    liked: true,
    count: 40,
    type: "/images/types/type6.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
]);
</script>
