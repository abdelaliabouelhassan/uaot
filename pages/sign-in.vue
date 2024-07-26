<template>
  <section class="pb-8 pt-28 h-full min-h-max">
    <div class="flex items-center max-w-[1237px] mx-auto px-4 gap-4">
      <div class="w-full hidden lg:block">
        <img
          src="/images/uaotdragon.png"
          class="w-full h-full object-cover"
          alt=""
        />
      </div>
      <!-- Login Form -->
      <div class="w-full max-w-[600px] space-y-4 mx-auto">
        <div class="bg-[#272727] w-full p-8 lg:p-14">
          <div class="flex flex-col items-center max-w-[550px] mx-auto gap-4">
            <h4
              class="text-[#D68637] font-assistant font-extrabold text-4xl pb-8"
            >
              SIGN IN
            </h4>

            <div class="relative w-full">
              <div class="absolute left-4 top-4">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 24 24"
                  fill="currentColor"
                  class="size-[19px] text-[#3F3F3F]"
                >
                  <path
                    d="M1.5 8.67v8.58a3 3 0 0 0 3 3h15a3 3 0 0 0 3-3V8.67l-8.928 5.493a3 3 0 0 1-3.144 0L1.5 8.67Z"
                  />
                  <path
                    d="M22.5 6.908V6.75a3 3 0 0 0-3-3h-15a3 3 0 0 0-3 3v.158l9.714 5.978a1.5 1.5 0 0 0 1.572 0L22.5 6.908Z"
                  />
                </svg>
              </div>
              <input
                type="text"
                class="bg-[#171717] py-3 outline-none placeholder-[#3F3F3F] text-[#FFDDBB] pl-10 text-lg pr-4 w-full"
                placeholder="E-Mail or Username"
              />
            </div>
            <div class="relative w-full">
              <div class="absolute left-4 top-4">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 24 24"
                  fill="currentColor"
                  class="size-[19px] text-[#3F3F3F]"
                >
                  <path
                    fill-rule="evenodd"
                    d="M12 1.5a5.25 5.25 0 0 0-5.25 5.25v3a3 3 0 0 0-3 3v6.75a3 3 0 0 0 3 3h10.5a3 3 0 0 0 3-3v-6.75a3 3 0 0 0-3-3v-3c0-2.9-2.35-5.25-5.25-5.25Zm3.75 8.25v-3a3.75 3.75 0 1 0-7.5 0v3h7.5Z"
                    clip-rule="evenodd"
                  />
                </svg>
              </div>
              <input
                type="text"
                class="bg-[#171717] py-3 outline-none placeholder-[#3F3F3F] text-[#FFDDBB] pl-10 text-lg pr-4 w-full"
                placeholder="Password"
              />
            </div>
            <div class="flex items-center w-full justify-between">
              <div class="flex items-center gap-2">
                <div class="inline-flex items-center">
                  <label
                    class="relative flex items-center rounded-full cursor-pointer"
                    htmlFor="checkbox"
                  >
                    <input
                      type="checkbox"
                      class="before:content[''] peer relative h-[33px] w-[33px] cursor-pointer appearance-none border-2 border-[#4E4E4E] transition-all before:absolute before:top-2/4 before:left-2/4 before:block before:h-12 before:w-12 before:-translate-y-2/4 before:-translate-x-2/4 before:rounded-full before:opacity-0 before:transition-opacity checked:border-gray-900 checked:bg-[#D68637] hover:before:opacity-10"
                      id="checkbox"
                      checked
                    />
                    <span
                      class="absolute text-white transition-opacity opacity-0 pointer-events-none top-2/4 left-2/4 -translate-y-2/4 -translate-x-2/4 peer-checked:opacity-100"
                    >
                      <svg
                        xmlns="http://www.w3.org/2000/svg"
                        class="h-3.5 w-3.5"
                        viewBox="0 0 20 20"
                        fill="currentColor"
                        stroke="currentColor"
                        stroke-width="1"
                      >
                        <path
                          fill-rule="evenodd"
                          d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                          clip-rule="evenodd"
                        ></path>
                      </svg>
                    </span>
                  </label>
                </div>
                <span class="text-[#FFDDBB] font-assistant">Remember me</span>
              </div>

              <div>
                <a href="#" class="text-[#D68637] font-assistant"
                  >Forgot password?</a
                >
              </div>
            </div>

            <div class="w-full pt-4">
              <button
                class="w-full text-[#FFDDBB] font-assistant font-extrabold text-xl md:text-4xl bg-[#D68637] text-center py-2 hover:scale-105 duration-200"
              >
                LOGIN
              </button>
            </div>

            <div class="w-full py-4 text-center">
              <span class="text-[#777777] font-assistant text-lg"
                >Or sign up using</span
              >
            </div>

            <div
              class="w-full flex flex-wrap sm:flex-nowrap items-center gap-5 lg:gap-10"
            >
              <button
                class="w-full rounded-full bg-[#7289DA] flex items-center py-2 justify-center gap-4 hover:scale-105 duration-200"
              >
                <div>
                  <img src="/images/discord.png" alt="" />
                </div>
                <span class="text-white font-assistant font-semibold text-xl"
                  >Discord</span
                >
              </button>
              <button
                class="w-full rounded-full bg-white flex items-center py-2 justify-center gap-4 hover:scale-105 duration-200"
              >
                <div>
                  <img src="/images/google.png" alt="" />
                </div>
                <span
                  class="text-[#272727] font-assistant font-semibold text-xl"
                  >Google</span
                >
              </button>
            </div>
          </div>
        </div>
        <p class="text-[#3F3F3F] font-assistant text-base">
          United Arts of Tyria will only store your email address and/or Discord
          ID to create and give you access to your user profile. We do not store
          any other personal data.
        </p>
      </div>
    </div>
  </section>
</template>

<script setup>
onMounted(() => {
  document.body.classList.toggle("bg-[#171717]");
});

onUnmounted(() => {
  document.body.classList.toggle("bg-[#171717]");
});
</script>
