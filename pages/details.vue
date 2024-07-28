<template>
  <div>
    <!-- Image -->
    <CollectiveDetails :items="Items" />
    <!-- About -->
    <AboutSection :about="About" />
  </div>
</template>

<script setup>
import CollectiveDetails from "@/components/partials/CollectiveDetails.vue";
import AboutSection from "@/components/partials/AboutSection.vue";
import ProfileCard from "@/components/UI/ProfileCard.vue";
import Label from "@/components/UI/Label.vue";
const About = ref({
  labels: [
    {
      text: "SYLVARI",
      bg: "#272727",
    },
    {
      text: "FEMALE",
      bg: "#272727",
    },
    {
      text: "LIGHT",
      bg: "#272727",
    },
    {
      text: "GREEN",
      bg: "#60814A",
    },
    {
      text: "PINK",
      bg: "#D8848E",
    },
    {
      text: "INFUSION",
      bg: "#272727",
    },
  ],
  content: `This is where it gets interesting. Aerial Finesse lets you
              wingflap during a dive (or a climb). We call this “boosting” or
              “speed-diving” since it gives you an extreme increase in speed and
              momentum. A properly executed boost will be visible by having
              yellow swirls around your Griffon (this does not apply to the
              “Nightfang” Griffon skin, since this one has them even when just
              regularly diving down).
              <br />
              <br />
              Most cosmetic infusions are a tied to extremely rare chance
              rewards from their relevant content. Sometimes they are not
              rewarded directly, and are
              <a href="#" class="underline">crafted</a> instead with the main
              crafting component being the rare drop. Some of these infusions
              can be obtained directly, avoiding the random drop mechanic and,
              partially, extremely high costs. This more direct way of
              acquisition usually comes with some restrictions.`,
});

const Items = ref({
  images: [
    "/images/Placeholder3.jpg",
    "/images/Placeholder6.jpg",
    "/images/Placeholder1.jpg",
  ],
  body: [
    {
      image: "/images/equipment_icons/Head_slot.png",
      colors: ["#FFC8E1", "#DC6E7B", "#C8A6AD", "#8DA27F"],
    },
    {
      image: "/images/equipment_icons/Shoulder_slot.png",
      colors: ["#FFC8E1", "#DC6E7B", "#C8A6AD"],
    },
    {
      image: "/images/equipment_icons/Chest_slot.png",
      colors: ["#FFC8E1", "#DC6E7B"],
    },
    {
      image: "/images/equipment_icons/Hand_slot.png",
      colors: ["#FFC8E1"],
    },
    {
      image: "/images/equipment_icons/Leg_slot.png",
      colors: ["#FFC8E1", "#DC6E7B", "#C8A6AD", "#8DA27F"],
    },
    {
      image: "/images/equipment_icons/Feet_slot.png",
      colors: ["#FFC8E1", "#DC6E7B", "#C8A6AD", "#8DA27F"],
    },
  ],
  equipments: [
    {
      image: "/images/equipment_icons/Mainhand_slot.png",
      infusion: "/images/equipment_icons/Infusion_slot.png",
    },
    {
      image: "/images/equipment_icons/Offhand_slot.png",
      infusion: "/images/equipment_icons/Infusion_slot.png",
    },
    {
      image: "/images/equipment_icons/Mainhand_slot.png",
      infusion: "/images/equipment_icons/Infusion_slot.png",
    },
    {
      image: "/images/equipment_icons/Offhand_slot.png",
      infusion: "/images/equipment_icons/Infusion_slot.png",
    },
  ],
});
</script>
