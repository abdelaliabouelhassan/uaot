<template>
  <div>
    <section class="bg-[#171717] py-8">
      <div class="w-full max-w-[1437px] mx-auto px-4">
        <div
          class="w-full flex lg:flex-row flex-col items-start gap-8 pt-6 justify-between"
        >
          <ProfileCard
            name="Nemain"
            ign="Nemain.5073"
            likes="275"
            images="36"
          />

          <Achievements />
        </div>
        <AboutMe :about="aboutme" />
      </div>
    </section>

    <section class="bg-[#272727] pt-6 pb-8 lg:pb-16">
      <div class="w-full max-w-[1437px] mx-auto px-4">
        <h3 class="font-assistant font-extrabold text-[#D68637] text-3xl">
          MY LOOKS
        </h3>
        <GridImages :images="Images" />
      </div>
    </section>
  </div>
</template>

<script setup>
import Pagination from "@/components/UI/Pagination.vue";
import GridImages from "@/components/UI/GridImages.vue";
import ProfileCard from "@/components/UI/ProfileCard.vue";
import Achievements from "@/components/partials/Achievements.vue";
import AboutMe from "@/components/partials/AboutMe.vue";

const aboutme =
  ref(`This is where it gets interesting. Aerial Finesse lets you wingflap during
      a dive (or a climb). We call this “boosting” or “speed-diving” since it
      gives you an extreme increase in speed and momentum. A properly executed
      boost will be visible by having yellow swirls around your Griffon (this
      does not apply to the “Nightfang” Griffon skin, since this one has them
      even when just regularly diving down).
      <br />
      <br />
      Most cosmetic infusions are a tied to extremely rare chance rewards from
      their relevant content. Sometimes they are not rewarded directly, and are
      <a href="#" class="underline">crafted</a> instead with the main crafting
      component being the rare drop. Some of these infusions can be obtained
      directly, avoiding the random drop mechanic and, partially, extremely high
      costs. This more direct way of acquisition usually comes with some
      restrictions.`);

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
    images: [
      "/images/Placeholder7.jpg",
      "/images/Placeholder1.png",
      "/images/Placeholder7.jpg",
      "/images/Placeholder2.jpg",
      "/images/Placeholder6.jpg",
      "/images/Placeholder7.jpg",
    ],
    liked: false,
    count: 15,
    type: "/images/types/type8.svg",
    title: "A Light in the Dark",
    name: "By Nemain",
  },
]);
</script>
