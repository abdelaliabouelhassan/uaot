<template>
  <section class="bg-[#272727] py-8">
    <div class="w-full max-w-[1437px] px-4 mx-auto">
      <h2 class="font-assistant font-extrabold text-[#D68637] text-2xl">
        SAKURA SYLVARI
      </h2>

      <div class="w-full flex lg:flex-row flex-col items-start gap-8 pt-6">
        <vueper-slides class="w-full h-[576px]" :fixed-height="true">
          <vueper-slide
            :image="item"
            v-for="(item, index, key) in items.images"
            :key="key"
          >
          </vueper-slide>
        </vueper-slides>

        <div
          class="w-full bg-[#171717] p-4 grid grid-cols-1 sm:grid-cols-2 gap-3 lg:max-w-[385px]"
        >
          <div class="grid md:grid-cols-2 lg:grid-cols-1 gap-2">
            <div
              class="flex items-start gap-2"
              v-for="(item, index, key) in items.body"
              :key="key"
            >
              <div class="w-[83px] h-[83px]">
                <img
                  :src="item.image"
                  class="w-full h-full object-cover"
                  alt=""
                />
              </div>
              <Colors :colors="item.colors" />
            </div>
          </div>
          <div class="grid md:grid-cols-2 lg:grid-cols-1 gap-2">
            <div
              class="flex items-start gap-2"
              v-for="(item, index, key) in items.equipments"
              :key="key"
            >
              <div class="w-[83px] h-[83px]">
                <img
                  :src="item.image"
                  class="w-full h-full object-cover"
                  alt=""
                />
              </div>
              <div class="w-[83px] h-[83px]">
                <img
                  :src="item.infusion"
                  class="w-full h-full object-cover"
                  alt=""
                />
              </div>
            </div>

            <div
              class="h-[83px] invisible"
              v-for="n in 6 - items.equipments.length"
              :key="n"
            ></div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { VueperSlides, VueperSlide } from "vueperslides";
import "vueperslides/dist/vueperslides.css";
import Colors from "@/components/UI/Colors.vue";
const props = defineProps(["items"]);
</script>
