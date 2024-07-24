<template>
  <section class="bg-[#272727] py-8">
    <div class="w-full max-w-[1437px] px-4 mx-auto">
      <h2 class="font-assistant font-extrabold text-[#D68637] text-2xl">
        SAKURA SYLVARI
      </h2>

      <div class="w-full flex lg:flex-row flex-col items-start gap-8 pt-6">
        <vueper-slides class="w-full h-[576px]" :fixed-height="true">
          <vueper-slide
            image="/images/Placeholder3.jpg"
            v-for="n in 4"
            :key="n"
          >
          </vueper-slide>
        </vueper-slides>

        <div
          class="w-full bg-[#171717] p-4 grid grid-cols-1 sm:grid-cols-2 gap-3 lg:max-w-[385px]"
        >
          <div class="grid md:grid-cols-2 lg:grid-cols-1 gap-2">
            <div class="flex items-start gap-2">
              <div class="w-[83px] h-[83px]">
                <img
                  src="/images/equipment_icons/Head_slot.png"
                  class="w-full h-full object-cover"
                  alt=""
                />
              </div>
              <div class="grid grid-cols-2 gap-1">
                <button class="w-[40px] h-[40px] bg-[#FFC8E1]"></button>
                <button class="w-[40px] h-[40px] bg-[#DC6E7B]"></button>
                <button class="w-[40px] h-[40px] bg-[#C8A6AD]"></button>
                <button class="w-[40px] h-[40px] bg-[#8DA27F]"></button>
              </div>
            </div>
            <div class="flex items-start gap-2">
              <div class="w-[83px] h-[83px]">
                <img
                  src="/images/equipment_icons/Shoulder_slot.png"
                  class="w-full h-full object-cover"
                  alt=""
                />
              </div>
              <div class="grid grid-cols-2 gap-1">
                <button class="w-[40px] h-[40px] bg-[#FFC8E1]"></button>
                <button class="w-[40px] h-[40px] bg-[#DC6E7B]"></button>
                <button class="w-[40px] h-[40px] bg-[#C8A6AD]"></button>
                <button class="w-[40px] h-[40px] bg-[#8DA27F]"></button>
              </div>
            </div>
            <div class="flex items-start gap-2">
              <div class="w-[83px] h-[83px]">
                <img
                  src="/images/equipment_icons/Chest_slot.png"
                  class="w-full h-full object-cover"
                  alt=""
                />
              </div>
              <div class="grid grid-cols-2 gap-1">
                <button class="w-[40px] h-[40px] bg-[#FFC8E1]"></button>
                <button class="w-[40px] h-[40px] bg-[#DC6E7B]"></button>
                <button class="w-[40px] h-[40px] bg-[#C8A6AD]"></button>
                <button class="w-[40px] h-[40px] bg-[#8DA27F]"></button>
              </div>
            </div>
            <div class="flex items-start gap-2">
              <div class="w-[83px] h-[83px]">
                <img
                  src="/images/equipment_icons/Hand_slot.png"
                  class="w-full h-full object-cover"
                  alt=""
                />
              </div>
              <div class="grid grid-cols-2 gap-1">
                <button class="w-[40px] h-[40px] bg-[#FFC8E1]"></button>
                <button class="w-[40px] h-[40px] bg-[#DC6E7B]"></button>
                <button class="w-[40px] h-[40px] bg-[#C8A6AD]"></button>
                <button class="w-[40px] h-[40px] bg-[#8DA27F]"></button>
              </div>
            </div>
            <div class="flex items-start gap-2">
              <div class="w-[83px] h-[83px]">
                <img
                  src="/images/equipment_icons/Leg_slot.png"
                  class="w-full h-full object-cover"
                  alt=""
                />
              </div>
              <div class="grid grid-cols-2 gap-1">
                <button class="w-[40px] h-[40px] bg-[#FFC8E1]"></button>
                <button class="w-[40px] h-[40px] bg-[#DC6E7B]"></button>
                <button class="w-[40px] h-[40px] bg-[#C8A6AD]"></button>
                <button class="w-[40px] h-[40px] bg-[#8DA27F]"></button>
              </div>
            </div>
            <div class="flex items-start gap-2">
              <div class="w-[83px] h-[83px]">
                <img
                  src="/images/equipment_icons/Feet_slot.png"
                  class="w-full h-full object-cover"
                  alt=""
                />
              </div>
              <div class="grid grid-cols-2 gap-1">
                <button class="w-[40px] h-[40px] bg-[#FFC8E1]"></button>
                <button class="w-[40px] h-[40px] bg-[#DC6E7B]"></button>
                <button class="w-[40px] h-[40px] bg-[#C8A6AD]"></button>
                <button class="w-[40px] h-[40px] bg-[#8DA27F]"></button>
              </div>
            </div>
          </div>
          <div class="grid md:grid-cols-2 lg:grid-cols-1 gap-2">
            <div class="flex items-start gap-2">
              <div class="w-[83px] h-[83px]">
                <img
                  src="/images/equipment_icons/Mainhand_slot.png"
                  class="w-full h-full object-cover"
                  alt=""
                />
              </div>
              <div class="w-[83px] h-[83px]">
                <img
                  src="/images/equipment_icons/Infusion_slot.png"
                  class="w-full h-full object-cover"
                  alt=""
                />
              </div>
            </div>
            <div class="flex items-start gap-2">
              <div class="w-[83px] h-[83px]">
                <img
                  src="/images/equipment_icons/Offhand_slot.png"
                  class="w-full h-full object-cover"
                  alt=""
                />
              </div>
              <div class="w-[83px] h-[83px]">
                <img
                  src="/images/equipment_icons/Infusion_slot.png"
                  class="w-full h-full object-cover"
                  alt=""
                />
              </div>
            </div>
            <div class="flex items-start gap-2">
              <div class="w-[83px] h-[83px]">
                <img
                  src="/images/equipment_icons/Mainhand_slot.png"
                  class="w-full h-full object-cover"
                  alt=""
                />
              </div>
              <div class="w-[83px] h-[83px]">
                <img
                  src="/images/equipment_icons/Infusion_slot.png"
                  class="w-full h-full object-cover"
                  alt=""
                />
              </div>
            </div>
            <div class="flex items-start gap-2">
              <div class="w-[83px] h-[83px]">
                <img
                  src="/images/equipment_icons/Offhand_slot.png"
                  class="w-full h-full object-cover"
                  alt=""
                />
              </div>
              <div class="w-[83px] h-[83px]">
                <img
                  src="/images/equipment_icons/Infusion_slot.png"
                  class="w-full h-full object-cover"
                  alt=""
                />
              </div>
            </div>
            <div class="flex items-start gap-2">
              <div class="w-[83px] h-[83px]">
                <img
                  src="/images/equipment_icons/Back_slot.png"
                  class="w-full h-full object-cover"
                  alt=""
                />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { VueperSlides, VueperSlide } from "vueperslides";
import "vueperslides/dist/vueperslides.css";
</script>
