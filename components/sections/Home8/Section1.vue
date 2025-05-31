<template>
  <swiper
    :direction="'vertical'"
    :pagination="{
      clickable: true,
    }"
    :modules="modules"
    class="mySwiper"
  >
    <div
      class="px-[12px] md:px-[36px] xl:px-0 mt-[70px] grid items-center mx-auto lg:mt-[128px] max-w-[1320px] lg:gap-10 lg:grid-cols-2 xl:grid-cols-[minmax(695px,_1fr)_1fr]"
    >
      <div class="flex-1">
        <span
          class="font-chivo inline-block bg-bg-6 text-green-900 py-[14px] px-[28px] rounded-[50px] text-[14px] leading-[14px] mb-[22px]"
          >ENVI-COMM CORPORATION</span
        >
        <h1
          class="font-chivo text-[35px] leading-[44px] sm:text-[46px] sm:leading-[52px] md:text-heading-1 font-extrabold mb-6 lg:mb-10"
        >
          <p class="font-bold inline-block">Leading &nbsp;</p>
          <p class="text-green-900 font-bold inline-block">
            Environmental&nbsp;
          </p>
          <p class="font-bold inline-block">Consultancy Solutions</p>
        </h1>
        <p class="text-quote md:text-lead-lg text-gray-600 mb-[45px]">
          we are a team of environmental experts dedicated to assisting
          businesses and organizations in navigating the complexities of
          environmental compliance
        </p>
      </div>
      <div class="items-center flex-1 relative hidden gap-[17px] lg:flex">
        <div class="flex-1 z-10">
          <img
            class="shadow-3 rounded-[158px] lg:max-w-[140px] xl:max-w-[184px]"
            src="/assets/images/hero-8a.png"
            alt="agon hero banner"
          />
        </div>
        <div class="flex-1 z-10">
          <img
            class="shadow-3 rounded-[158px] lg:max-w-[140px] xl:max-w-[184px]"
            src="/assets/images/hero-8b.png"
            alt="agon hero banner"
          />
        </div>
        <div class="flex-1 z-10">
          <img
            class="shadow-3 rounded-[158px] lg:max-w-[140px] xl:max-w-[184px]"
            src="/assets/images/hero-8c.png"
            alt="agon hero banner"
          />
        </div>
        <div
          class="rounded-full absolute opacity-50 w-[600px] h-[600px] bg-[#9BE9FB] blur-[200px] z-0 top-0 left-0 -translate-x-1/3 -translate-y-1/3"
        ></div>
        <div
          class="rounded-full absolute opacity-50 w-[400px] h-[400px] bg-[#FFD5C8] blur-[200px] z-0 bottom-0 right-0 translate-x-1/3 translate-y-1/3"
        ></div>
      </div>
    </div>
  </swiper>
</template>

<script>
import { Swiper, SwiperSlide } from "swiper/vue";

import "swiper/css";
import "swiper/css/pagination";

import { Pagination } from "swiper/modules";
export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Pagination],
    };
  },
};
</script>