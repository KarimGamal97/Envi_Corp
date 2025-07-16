<template>
    <swiper
        :slides-per-view="1"
        :space-between="0"
        :loop="true"
        :autoplay="{
            delay: 3000,
            disableOnInteraction: true,
        }"
        :pagination="{
            el: '.swiper-pagination',
            clickable: true,
        }"
        :navigation="{
            nextEl: '.tan1',
            prevEl: '.tap1',
        }"
        :modules="modules"
        class="feedback-list ml-[-15px]"
    >
        <swiper-slide
            class="p-10 transition-all duration-300 border-[10px] mx-[15px] hover:translate-y-[-2px] mt-[2px] border-bg-2"
        >
            <img
                src="/assets/images/main-imgs/rating.png"
                alt="rating-stars"
                class="w-[200px] mb-5"
            />

            <p class="text-lg md:text-xl text-gray-500 uppercase mb-5">
                "I am very satisfied with the service provided by Envi-comm. The quality of their
                work is excellent, and both the staff and team leader are highly professional in
                their respective fields.”Even factoring differences in body weight between children
                and adults into account.
            </p>
            <img
                class="h-full w-full object-cover max-w-[55px] max-h-[55px] mb-[22px] drop-shadow-md rounded-full"
                src="/assets/images/main-imgs/logo-01.png"
                alt="avatar"
            />
            <p class="text-heading-6 font-poppins font-bold mb-[6px]">
                EASTLAND PROPERTY VENTURES, INC
            </p>
            <p class="text-sm md:text-md font-semibold text-gray-700">
                Proposed 10-Storey Socialized Condominium Development
            </p>
        </swiper-slide>
        <swiper-slide
            class="p-10 transition-all duration-300 border-[10px] mx-[15px] hover:translate-y-[-2px] mt-[2px] border-bg-2"
        >
            <img
                src="/assets/images/main-imgs/rating.png"
                alt="rating-stars"
                class="w-[200px] mb-5"
            />

            <p class="text-lg md:text-xl text-gray-500 uppercase mb-5">
                “We are very satisfied with your service, and if I'm going to rate it from 1 to 10,
                it is always 10.”
            </p>
            <img
                class="h-full w-full object-cover max-w-[55px] max-h-[55px] mb-[22px] drop-shadow-md rounded-full"
                src="/assets/images/main-imgs/logo-02.png"
                alt="avatar"
            />
            <p class="text-heading-6 font-poppins font-bold mb-[6px]">HAGNAYA BEACH RESORT</p>
            <p class="text-sm md:text-md font-semibold text-gray-700">Beach Resort Project</p>
        </swiper-slide>
        <swiper-slide
            class="p-10 transition-all duration-300 border-[10px] mx-[15px] hover:translate-y-[-2px] mt-[2px] border-bg-2"
        >
            <img
                src="/assets/images/main-imgs/rating.png"
                alt="rating-stars"
                class="w-[200px] mb-5"
            />
            <p class="text-lg md:text-xl text-gray-500 uppercase mb-5">
                "So far, I love the service here at Envi-comm Corporation, and I can truly say that
                their service is excellent."
            </p>
            <img
                class="h-full w-full object-cover max-w-[55px] max-h-[55px] mb-[22px] drop-shadow-md rounded-full"
                src="/assets/images/main-imgs/logo-03.png"
                alt="avatar"
            />
            <p class="text-heading-6 font-poppins font-bold mb-[6px]">
                SHEMBERG-INGREDIENTS GUMS AND CORPORATION
            </p>
            <p class="text-sm md:text-md font-semibold text-gray-700">
                SHEMBERG-INGREDIENTS GUMS AND CORPORATION
            </p>
        </swiper-slide>
    </swiper>
</template>
<script>
import { Autoplay, Navigation, Pagination } from "swiper/modules";
import { Swiper, SwiperSlide } from "swiper/vue";
import "swiper/css";

export default {
    components: {
        Swiper,
        SwiperSlide,
    },
    setup() {
        return {
            modules: [Autoplay, Pagination, Navigation],
        };
    },
};
</script>
