<template>
  <section class="bg-[#171717] pt-8 pb-44">
    <div class="w-full max-w-[1437px] mx-auto px-4">
      <div class="w-full flex lg:flex-row flex-col items-start gap-8 pt-6">
        <div class="w-full space-y-4 pr-8 order-3 lg:order-1">
          <h2 class="font-assistant font-extrabold text-[#D68637] text-2xl">
            ABOUT THIS LOOK
          </h2>

          <div class="flex flex-wrap gap-3 items-start">
            <Label
              :text="lable.text"
              :bg="lable.bg"
              v-for="(lable, key) in about.labels"
              :key="key"
            />
          </div>

          <p
            class="font-assistant text-[#FFDDBB] text-base"
            v-html="about.content"
          ></p>
        </div>
        <div
          class="border border-[#3F3F3F] w-[241px] lg:w-0 lg:h-[241px] order-2"
        ></div>
        <div class="w-full max-w-[385px] space-y-4 order-1 lg:order-3">
          <h2 class="font-assistant font-extrabold text-[#D68637] text-2xl">
            LOOK BY
          </h2>

          <ProfileCard
            name="Nemain"
            ign="Nemain.5073"
            likes="275"
            images="36"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import ProfileCard from "@/components/UI/ProfileCard.vue";
import Label from "@/components/UI/Label.vue";
const props = defineProps(["about"]);
</script>
