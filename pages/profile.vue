<template>
  <div>
    <section class="bg-[#171717] py-8">
      <div class="w-full max-w-[1437px] mx-auto px-4">
        <div
          class="w-full flex lg:flex-row flex-col items-start gap-8 pt-6 justify-between"
        >
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
                Nemain
              </h4>
              <span class="text-[#FFDDBB] font-assistant font-normal text-lg"
                >IGN: Nemain.5073</span
              >

              <div class="flex items-center gap-4">
                <div class="flex items-center gap-2">
                  <img
                    src="/images/icons/active-heart.svg"
                    class="w-[19px] h-[19px] object-cover"
                    alt=""
                  />
                  <span
                    class="text-[#FFDDBB] font-assistant font-normal text-lg"
                    >275</span
                  >
                </div>
                <div class="flex items-center gap-2">
                  <img
                    src="/images/icons/shirt.png"
                    class="w-[19px] h-[19px] object-cover"
                    alt=""
                  />
                  <span
                    class="text-[#FFDDBB] font-assistant font-normal text-lg"
                    >36</span
                  >
                </div>
              </div>
            </div>
          </div>

          <div class="flex flex-col items-start gap-4">
            <h2 class="font-assistant font-extrabold text-[#D68637] text-3xl">
              ACHIEVEMENTS
            </h2>
            <div class="flex items-start flex-wrap gap-3">
              <div
                class="w-[80px] h-[80px] rounded-full bg-[#FFDDBB]"
                v-for="n in 4"
                :key="n"
              ></div>
              <div
                class="w-[80px] h-[80px] rounded-full border-2 border-[#D68637] flex"
              >
                <span class="m-auto text-[#FFDDBB] text-4xl font-assistant"
                  >+ 5</span
                >
              </div>
            </div>
          </div>
        </div>
        <div class="w-full space-y-4 pt-10">
          <h3 class="font-assistant font-extrabold text-[#D68637] text-3xl">
            ABOUT ME
          </h3>

          <p class="font-assistant text-[#FFDDBB] text-base">
            This is where it gets interesting. Aerial Finesse lets you wingflap
            during a dive (or a climb). We call this “boosting” or
            “speed-diving” since it gives you an extreme increase in speed and
            momentum. A properly executed boost will be visible by having yellow
            swirls around your Griffon (this does not apply to the “Nightfang”
            Griffon skin, since this one has them even when just regularly
            diving down).
            <br />
            <br />
            Most cosmetic infusions are a tied to extremely rare chance rewards
            from their relevant content. Sometimes they are not rewarded
            directly, and are
            <a href="#" class="underline">crafted</a> instead with the main
            crafting component being the rare drop. Some of these infusions can
            be obtained directly, avoiding the random drop mechanic and,
            partially, extremely high costs. This more direct way of acquisition
            usually comes with some restrictions.
          </p>
        </div>
      </div>
    </section>

    <section class="bg-[#272727] pt-6 pb-8 lg:pb-16">
      <div class="w-full max-w-[1437px] mx-auto px-4">
        <h3 class="font-assistant font-extrabold text-[#D68637] text-3xl">
          MY LOOKS
        </h3>
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
        <div class="w-full flex justify-end pt-4 lg:pt-0">
          <Pagination />
        </div>
      </div>
    </section>
  </div>
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
