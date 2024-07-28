<template>
  <form class="flex md:justify-end w-full pb-4">
    <div class="flex md:flex-row flex-col items-start gap-4 w-full md:w-fit">
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
</template>
