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

      <div class="w-full max-w-[600px] space-y-4 mx-auto">
        <div class="bg-[#272727] w-full p-8 lg:p-14">
          <div class="flex flex-col items-center max-w-[550px] mx-auto gap-4">
            <h4
              class="text-[#D68637] font-assistant font-extrabold text-4xl pb-4"
            >
              CREATE NEW ACCOUNT
            </h4>
            <p class="text-[#FFDDBB] font-assistant text-lg">
              There currently exists no account with that E-Mail adress.
              <br /><br />
              Would you like to continue and create a new account registered to
              that adress?
            </p>
            <div class="w-full pt-4 flex flex-col gap-4">
              <nuxt-link to="sign-in">
                <button
                  class="w-full text-[#FFDDBB] font-assistant font-extrabold text-xl md:text-4xl bg-[#171717] border border-[#3F3F3F] text-center py-2 hover:scale-105 duration-200"
                >
                  GO BACK
                </button>
              </nuxt-link>
              <nuxt-link to="sign-in">
                <button
                  class="w-full text-[#FFDDBB] font-assistant font-extrabold text-xl md:text-4xl bg-[#D68637] text-center py-2 hover:scale-105 duration-200"
                >
                  CREATE ACCOUNT
                </button>
              </nuxt-link>
            </div>
          </div>
        </div>
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
