<template>
  <div class="bg-[#272727] pt-6">
    <div class="w-full max-w-[1437px] mx-auto px-4 space-y-4">
      <div class="flex justify-end w-full">
        <div class="flex items-start gap-4">
          <div class="flex flex-col items-start gap-1">
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
          <div class="flex flex-col items-start gap-1">
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
          <div class="flex flex-col items-start gap-1">
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
          <div class="flex flex-col items-start gap-1">
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
          <div class="flex flex-col items-start gap-1">
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
          <div class="flex flex-col items-start gap-1">
            <label
              for="search"
              class="text-[#D68637] font-bold font-assistant text-sm"
              >KEYWORD SEARCH</label
            >
            <div class="relative">
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
                class="bg-[#171717] py-3 outline-none placeholder-[#3F3F3F] text-[#FFDDBB] pl-8 text-sm"
                placeholder="KEYWORD OR USER"
              />
            </div>
          </div>
        </div>
      </div>

      <div class="w-full border-[0.5px] border-[#83838363]"></div>

      <div class="w-full grid grid-cols-4 gap-4">
        <div class="w-full h-[641px] bg-gray-400">
          <img
            src="/images/Placeholder1.jpg"
            class="w-full h-full object-cover"
            alt=""
          />
        </div>
        <div class="w-full h-[641px] bg-gray-400"></div>
      </div>
    </div>
  </div>
</template>
