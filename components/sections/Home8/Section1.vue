<template>
    <section id="section1" class="w-full min-h-[calc(100dvh-85px)] md:min-h-[calc(100vh-95px)]">
        <Swiper
            @swiper="onSwiper"
            :modules="modules"
            :slides-per-view="1"
            :space-between="0"
            :loop="true"
            :pagination="{
                clickable: false,
                el: '.swiper-pagination',
            }"
            :navigation="{
                nextEl: '.swiper-button-next',
                prevEl: '.swiper-button-prev',
            }"
            :autoplay="{
                delay: 5000,
                disableOnInteraction: false,
            }"
            class="mySwiper min-h-[calc(100dvh-85px)] md:min-h-[calc(100vh-95px)] w-full relative overflow-hidden"
        >
            <!-- Slide 1 -->
            <SwiperSlide class="min-h-[calc(100dvh-85px)] md:min-h-[calc(100vh-95px)] w-full">
                <div
                    class="relative w-full min-h-[calc(100dvh-85px)] md:min-h-[calc(100vh-95px)] bg-contain bg-top md:bg-cover md:bg-center bg-no-repeat bg-[url('/assets/images/main-imgs/slider-01-phone.jpg')] md:bg-[url('/assets/images/main-imgs/slider-01.jpg')]"
                >
                    <div
                        class="relative z-10 pb-5 px-5 md:px-20 flex flex-col justify-end text-center md:text-start md:justify-center gap-5 min-h-[calc(100dvh-85px)] md:min-h-[calc(100vh-95px)]"
                    >
                        <h2 class="text-3xl md:text-4xl font-semibold text-black md:max-w-[40%]">
                            STP & WTP SYSTEMS Engineered for Efficiency
                        </h2>
                        <p class="text-black text-clamp md:max-w-[25%]">
                            One-stop solutions for effective wastewater and water treatment with
                            minimal downtime and maximum performance.
                        </p>
                        <button
                            class="bg-[#547326] border-2 border-white text-clamp rounded-md text-white px-5 py-2 w-fit mx-auto block md:mx-0"
                        >
                            Know More
                        </button>
                    </div>
                </div>
            </SwiperSlide>

            <!-- Slide 2 -->
            <SwiperSlide class="min-h-[calc(100dvh-85px)] md:min-h-[calc(100vh-95px)] w-full">
                <div
                    class="relative w-full min-h-[calc(100dvh-85px)] md:min-h-[calc(100vh-95px)] bg-contain bg-top md:bg-cover md:bg-center bg-no-repeat bg-[url('/assets/images/main-imgs/slider-02-phone.jpg')] md:bg-[url('/assets/images/main-imgs/slider-02.jpg')]"
                >
                    <div
                        class="relative z-10 py-10 px-5 md:px-20 flex flex-col justify-end text-center md:text-start md:justify-center gap-5 min-h-[calc(100dvh-85px)] md:min-h-[calc(100vh-95px)]"
                    >
                        <h2
                            class="text-3xl md:text-4xl font-semibold text-black md:text-white md:max-w-[35%]"
                        >
                            EIS Tailored for Your Industry
                        </h2>
                        <p class="text-clamp text-black md:text-white md:max-w-[25%]">
                            Whether infrastructure, energy, or development — our Environmental
                            Impact Studies are built to match your sector's needs.
                        </p>
                        <button
                            class="bg-[#547326] border-2 border-white text-clamp rounded-md text-white px-5 py-2 w-fit mx-auto block md:mx-0"
                        >
                            Know More
                        </button>
                    </div>
                </div>
            </SwiperSlide>

            <!-- Slide 3 -->
            <SwiperSlide class="min-h-[calc(100dvh-85px)] md:min-h-[calc(100vh-95px)] w-full">
                <div
                    class="relative w-full min-h-[calc(100dvh-85px)] md:min-h-[calc(100vh-95px)] bg-contain bg-top md:bg-cover md:bg-center bg-no-repeat bg-[url('/assets/images/main-imgs/slider-03-phone.jpg')] md:bg-[url('/assets/images/main-imgs/slider-03.jpg')]"
                >
                    <div
                        class="relative z-10 pb-5 px-5 md:px-20 flex flex-col justify-end text-center md:text-start md:justify-center md:gap-5 min-h-[calc(100dvh-85px)] md:min-h-[calc(100vh-95px)]"
                    >
                        <h2
                            class="text-2xl md:text-4xl font-semibold mb-5 text-black md:max-w-[30%]"
                        >
                            Solar Streetlight That Saves More Than Just Power
                        </h2>
                        <p class="text-black text-clamp mb-5 md:max-w-[30%]">
                            Introducing our 150W Solar Streetlight Harness the sun to save
                            electricity, cut carbon emissions, and protect the planet — without
                            compromising brightness or reliability.
                        </p>
                        <button
                            class="bg-[#547326] border-2 border-white text-clamp rounded-md text-white px-5 py-2 w-fit mx-auto block md:mx-0"
                        >
                            Know More
                        </button>
                    </div>
                </div>
            </SwiperSlide>

            <!-- Slide 4 -->
            <SwiperSlide class="min-h-[calc(100dvh-85px)] md:min-h-[calc(100vh-95px)] w-full">
                <div
                    class="relative w-full min-h-[calc(100dvh-85px)] md:min-h-[calc(100vh-95px)] bg-contain bg-top md:bg-cover md:bg-center bg-no-repeat bg-[url('/assets/images/main-imgs/slider-04-phone.jpg')] md:bg-[url('/assets/images/main-imgs/slider-04.jpg')]"
                >
                    <div
                        class="relative z-10 pb-10 px-5 md:px-20 flex flex-col justify-end text-center md:text-start md:justify-center gap-5 min-h-[calc(100dvh-85px)] md:min-h-[calc(100vh-95px)]"
                    >
                        <h2
                            class="text-3xl md:text-4xl font-semibold mb-10 text-black md:text-white md:max-w-[30%]"
                        >
                            Secure Your DENR Certificate of Tree Planting
                        </h2>
                        <button
                            class="text-clamp bg-transparent border-2 border-black md:border-white rounded-md text-black md:text-white px-5 py-2 w-fit mx-auto block md:mx-0"
                        >
                            Know More
                        </button>
                    </div>
                </div>
            </SwiperSlide>

            <!-- Slide 5 -->
            <SwiperSlide class="min-h-[calc(100dvh-85px)] md:min-h-[calc(100vh-95px)] w-full">
                <div
                    class="relative w-full min-h-[calc(100dvh-85px)] md:min-h-[calc(100vh-95px)] bg-contain bg-top md:bg-cover md:bg-center bg-no-repeat bg-[url('/assets/images/main-imgs/slider-05-phone.jpg')] md:bg-[url('/assets/images/main-imgs/slider-05.jpg')]"
                >
                    <div
                        class="relative z-10 pb-10 px-5 md:px-20 flex flex-col justify-end text-center md:text-start md:justify-center md:gap-5 min-h-[calc(100dvh-85px)] md:min-h-[calc(100vh-95px)]"
                    >
                        <h2
                            class="text-2xl md:text-4xl font-semibold mb-5 text-black md:max-w-[35%]"
                        >
                            Compliance Made Simple. Savings Made Easy.
                        </h2>
                        <p class="text-black text-clamp mb-5 md:max-w-[25%]">
                            Envi-comm’s Retainership Program gives you continuous support and peace
                            of mind, so you can run your business worry-free.
                        </p>
                        <button
                            class="bg-[#547326] border-2 border-white text-clamp rounded-md text-white px-5 py-2 w-fit mx-auto block md:mx-0"
                        >
                            Know More
                        </button>
                    </div>
                </div>
            </SwiperSlide>

            <!-- Slide 6 -->
            <SwiperSlide class="min-h-[calc(100dvh-85px)] md:min-h-[calc(100vh-95px)] w-full">
                <div
                    class="relative w-full min-h-[calc(100dvh-85px)] md:min-h-[calc(100vh-95px)] bg-contain bg-top md:bg-cover md:bg-center bg-no-repeat bg-[url('/assets/images/main-imgs/slider-06-phone.jpg')] md:bg-[url('/assets/images/main-imgs/slider-06.jpg')]"
                >
                    <div
                        class="relative z-10 pb-10 px-5 md:px-20 flex flex-col justify-end text-center md:text-start md:justify-center md:gap-5 min-h-[calc(100dvh-85px)] md:min-h-[calc(100vh-95px)]"
                    >
                        <h2
                            class="text-2xl md:text-4xl font-semibold mb-5 text-black md:max-w-[35%]"
                        >
                            Clean Water Starts with Proven Chemistry
                        </h2>
                        <p class="text-black text-clamp mb-5 md:max-w-[25%]">
                            Envi-comm Corporation provides high-performance chemical solutions
                            tailored for optimal sludge control, odor management, and regulatory
                            compliance.
                        </p>
                        <button
                            class="bg-[#547326] border-2 border-white text-clamp rounded-md text-white px-5 py-2 w-fit mx-auto block md:mx-0"
                        >
                            Know More
                        </button>
                    </div>
                </div>
            </SwiperSlide>

            <!-- Navigation Buttons -->
            <div class="hidden md:block">
                <div class="swiper-button-next"></div>
                <div class="swiper-button-prev"></div>
            </div>

            <!-- Pagination -->
            <div class="swiper-pagination hidden"></div>
        </Swiper>

        <!-- Slide titles under the slider -->
        <div class="bg-[#1C1C1C] py-2">
            <div class="container">
                <div class="flex justify-between gap-1 md:gap-3">
                    <button
                        v-for="(title, index) in slideTitles"
                        :key="index"
                        @click="goToSlide(index)"
                        :class="[
                            'text-[10px] md:text-md 3xl:text-lg transition-all duration-200 uppercase hover:underline',
                            currentSlideIndex === index
                                ? 'font-semibold text-white'
                                : 'text-gray-200',
                        ]"
                    >
                        {{ title }}
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- <section id="section2">
        <div class="px-[12px] md:px-[36px] xl:px-0 mt-[70px] lg:mt-[150px]">
            <span
                class="font-poppins inline-block bg-bg-2 text-green-900 py-[14px] px-[28px] rounded-[50px] text-[14px] leading-[14px] mb-8"
                >Company Overview</span
            >
            <div class="mb-14">
                <h2
                    class="text-gray-900 font-bold font-poppins mb-5 text-[35px] leading-[44px] md:text-[46px] md:leading-[52px] lg:text-heading-1 md:mb-[30px] max-w-[725px]"
                >
                    Envi-Comm Corporation
                </h2>
                <p class="text-quote md:text-lead-lg text-gray-600">
                    We are a team of environmental experts dedicated to assisting businesses.
                </p>
            </div>
            <div
                class="grid grid-cols-1 md:grid-cols-2 xl:grid-cols-3 gap-x-[30px] gap-y-[50px] mb-[52px]"
            >
                <div class="rounded-2xl p-[25px] pb-[35px] border border-gray-200">
                    <div class="aspect-[408/275]">
                        <img
                            class="min-h-[calc(100dvh-85px)] md:min-h-[calc(100vh-95px)] w-full object-cover rounded-2xl mb-[30px]"
                            src="/assets/images/destination-1.png"
                            alt="Img"
                        />
                    </div>
                    <div class="flex items-center gap-[10px] mb-[11px]"></div>
                    <h4
                        class="font-bold font-poppins text-[14px] xl:text-heading-5 mb-[15px] text-center"
                    >
                        Application
                    </h4>
                    <p class="text-text text-gray-500 text-center">
                        Streamlining the environmental application process for our clients to ensure
                        compliance and expedite project approvals.
                    </p>
                </div>
                <div class="rounded-2xl p-[25px] pb-[35px] border border-gray-200">
                    <div class="aspect-[408/275]">
                        <img
                            class="min-h-[calc(100dvh-85px)] md:h-screen w-full object-cover rounded-2xl mb-[30px]"
                            src="/assets/images/destination-1.png"
                            alt="Img"
                        />
                    </div>
                    <div class="flex items-center gap-[10px] mb-[11px]"></div>
                    <h4
                        class="font-bold font-poppins text-[14px] xl:text-heading-5 mb-[15px] text-center"
                    >
                        Application
                    </h4>
                    <p class="text-text text-gray-500 text-center">
                        Streamlining the environmental application process for our clients to ensure
                        compliance and expedite project approvals.
                    </p>
                </div>
                <div class="rounded-2xl p-[25px] pb-[35px] border border-gray-200">
                    <div class="aspect-[408/275]">
                        <img
                            class="h-full w-full object-cover rounded-2xl mb-[30px]"
                            src="/assets/images/destination-1.png"
                            alt="Img"
                        />
                    </div>
                    <div class="flex items-center gap-[10px] mb-[11px]"></div>
                    <h4
                        class="font-bold font-poppins text-[14px] xl:text-heading-5 mb-[15px] text-center"
                    >
                        Application
                    </h4>
                    <p class="text-text text-gray-500 text-center">
                        Streamlining the environmental application process for our clients to ensure
                        compliance and expedite project approvals.
                    </p>
                </div>
            </div>
            <button type="button">
                <NuxtLink
                    class="flex items-center z-10 relative transition-all duration-200 group px-[22px] py-[15px] lg:px-[32px] lg:py-[22px] rounded-[50px] bg-gray-900 text-white hover:bg-gray-100 hover:text-gray-900 mx-auto tracking-wide text-md w-fit gap-4 md:text-heading-6"
                    to="#"
                    ><span
                        class="block text-inherit w-full h-full rounded-[50px] text-lg font-poppins font-semibold"
                        >Discover More</span
                    ><i>
                        <img
                            class="ml-[7px] w-[12px] filter-white group-hover:filter-black"
                            src="/assets/images/icons/icon-right.svg"
                            alt="arrow right icon"
                            to="/about" /></i
                ></NuxtLink>
            </button>
        </div>
    </section> -->
    <section id="section3" class="py-20">
        <div class="container">
            <h2
                class="text-center text-gray-900 uppercase font-poppins mb-5 text-[35px] leading-[44px] md:text-[46px] lg:text-heading-1 md:mb-[30px]"
                data-aos="fade-up"
            >
                What We Do
            </h2>
            <div class="grid grid-cols-1 md:grid-cols-2 xl:grid-cols-3 gap-5">
                <!-- items 1 -->
                <div class="relative rounded-lg overflow-hidden h-[150px] group" data-aos="fade-up">
                    <div
                        class="absolute inset-0 bg-black/40 hover:bg-[#547326]/40 transition-all duration-300 w-full h-full"
                    ></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_01.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3
                        class="text-white border-b-[1.5px] border-white pb-1 text-clamp absolute bottom-10 left-10"
                    >
                        Planning
                    </h3>
                </div>
                <!-- items 2 -->
                <div
                    class="relative rounded-lg overflow-hidden h-[150px] group"
                    data-aos="fade-up"
                    data-aos-delay="300"
                >
                    <div
                        class="absolute inset-0 bg-black/40 hover:bg-[#547326]/40 transition-all duration-300 w-full h-full"
                    ></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_02.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3
                        class="text-white border-b-[1.5px] border-white pb-1 text-clamp absolute bottom-10 left-10"
                    >
                        Permitting
                    </h3>
                </div>
                <!-- items 3 -->
                <div class="relative rounded-lg overflow-hidden h-[150px] group" data-aos="fade-up">
                    <div
                        class="absolute inset-0 bg-black/40 hover:bg-[#547326]/40 transition-all duration-300 w-full h-full"
                    ></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_03.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3
                        class="text-white border-b-[1.5px] border-white pb-1 text-clamp absolute bottom-10 left-10"
                    >
                        Reporting
                    </h3>
                </div>
                <!-- items 4 -->
                <div
                    class="relative rounded-lg overflow-hidden h-[150px] group"
                    data-aos="fade-up"
                    data-aos-delay="600"
                >
                    <div
                        class="absolute inset-0 bg-black/40 hover:bg-[#547326]/40 transition-all duration-300 w-full h-full"
                    ></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_04.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3
                        class="text-white border-b-[1.5px] border-white pb-1 text-clamp absolute bottom-10 left-10"
                    >
                        STPs
                    </h3>
                </div>
                <!-- items 5 -->
                <div
                    class="relative rounded-lg overflow-hidden h-[150px] group"
                    data-aos="fade-up"
                    data-aos-delay="300"
                >
                    <div
                        class="absolute inset-0 bg-black/40 hover:bg-[#547326]/40 transition-all duration-300 w-full h-full"
                    ></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_05.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3
                        class="text-white border-b-[1.5px] border-white pb-1 text-clamp absolute bottom-10 left-10"
                    >
                        STP Chemicals
                    </h3>
                </div>
                <!-- items 6 -->
                <div
                    class="relative rounded-lg overflow-hidden h-[150px] group"
                    data-aos="fade-up"
                    data-aos-delay="600"
                >
                    <div
                        class="absolute inset-0 bg-black/40 hover:bg-[#547326]/40 transition-all duration-300 w-full h-full"
                    ></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_06.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3
                        class="text-white border-b-[1.5px] border-white pb-1 text-clamp absolute bottom-10 left-10"
                    >
                        Solar
                    </h3>
                </div>
                <!-- items 7 -->
                <div
                    class="relative rounded-lg overflow-hidden h-[150px] group"
                    data-aos="fade-up"
                    data-aos-delay="600"
                >
                    <div
                        class="absolute inset-0 bg-black/40 hover:bg-[#547326]/40 transition-all duration-300 w-full h-full"
                    ></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_07.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3
                        class="text-white border-b-[1.5px] border-white pb-1 text-clamp absolute bottom-10 left-10"
                    >
                        Hauling & Septage
                    </h3>
                </div>
                <!-- items 8 -->
                <div
                    class="relative rounded-lg overflow-hidden h-[150px] group"
                    data-aos="fade-up"
                    data-aos-delay="600"
                >
                    <div
                        class="absolute inset-0 bg-black/40 hover:bg-[#547326]/40 transition-all duration-300 w-full h-full"
                    ></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_08.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3
                        class="text-white border-b-[1.5px] border-white pb-1 text-clamp absolute bottom-10 left-10"
                    >
                        Saas
                    </h3>
                </div>
                <!-- items 9 -->
                <div
                    class="relative rounded-lg overflow-hidden h-[150px] group"
                    data-aos="fade-up"
                    data-aos-delay="600"
                >
                    <div
                        class="absolute inset-0 bg-black/40 hover:bg-[#547326]/40 transition-all duration-300 w-full h-full"
                    ></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_09.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3
                        class="text-white border-b-[1.5px] border-white pb-1 text-clamp absolute bottom-10 left-10"
                    >
                        Training
                    </h3>
                </div>
                <!-- items 10 -->
                <div
                    class="relative rounded-lg overflow-hidden h-[150px] group opacity-0 hidden md:block"
                >
                    <div
                        class="absolute inset-0 bg-black/40 hover:bg-[#547326]/40 transition-all duration-300 w-full h-full"
                    ></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_10.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3
                        class="text-white border-b-[1.5px] border-white pb-1 text-clamp absolute bottom-10 left-10"
                    >
                        Planning
                    </h3>
                </div>
                <!-- items 10 -->
                <div
                    class="relative rounded-lg overflow-hidden h-[150px] group"
                    data-aos="fade-up"
                    data-aos-delay="600"
                >
                    <div
                        class="absolute inset-0 bg-black/40 hover:bg-[#547326]/40 transition-all duration-300 w-full h-full"
                    ></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_10.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3
                        class="text-white border-b-[1.5px] border-white pb-1 text-clamp absolute bottom-10 left-10"
                    >
                        Planning
                    </h3>
                </div>
                <!-- items 10 -->
                <div
                    class="relative rounded-lg overflow-hidden h-[150px] group opacity-0 hidden md:block"
                >
                    <div
                        class="absolute inset-0 bg-black/40 hover:bg-[#547326]/40 transition-all duration-300 w-full h-full"
                    ></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_10.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3
                        class="text-white border-b-[1.5px] border-white pb-1 text-clamp absolute bottom-10 left-10"
                    >
                        Planning
                    </h3>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import { Swiper, SwiperSlide } from "swiper/vue";
import { Navigation, Pagination, Autoplay } from "swiper/modules";
import "swiper/css";
import "swiper/css/navigation";
import "swiper/css/pagination";

export default {
    components: {
        Swiper,
        SwiperSlide,
    },
    data() {
        return {
            swiperInstance: null,
            currentSlideIndex: 0,
            slideTitles: [
                "STP / WTP",
                "ECC: EIS",
                "SOLAR",
                "ECC: TREE PLANTING",
                "ECC: IEE",
                "CHEMICALS",
            ],
            modules: [Navigation, Pagination, Autoplay],
        };
    },
    methods: {
        onSwiper(swiper) {
            this.swiperInstance = swiper;

            swiper.on("slideChange", () => {
                this.currentSlideIndex = swiper.realIndex;
            });
        },
        goToSlide(index) {
            if (this.swiperInstance) {
                this.swiperInstance.slideToLoop(index);
            } else {
                console.warn("Swiper instance not ready");
            }
        },
        scrollToSection(index) {
            this.isScrolling = true;
            const targetSection = this.sections[index];
            if (!targetSection) return;

            window.scrollTo({
                top: targetSection.offsetTop - 60,
                behavior: "smooth",
            });

            setTimeout(() => {
                this.currentSection = index;
                this.isScrolling = false;
            }, 1600);
        },

        updateCurrentSection() {
            const scrollY = window.scrollY + window.innerHeight / 2;

            this.sections.forEach((section, index) => {
                const top = section.offsetTop;
                const height = section.offsetHeight;

                if (scrollY >= top && scrollY < top + height) {
                    this.currentSection = index;
                }
            });
        },
    },
    mounted() {
        this.$nextTick(() => {
            this.swiperInstance = this.$refs.mySwiper.swiper;
        });

        // Define the scroll handler function
        this.sections = Array.from(document.querySelectorAll("section[id^='section']"));
        this.currentSection = 0;
        this.isScrolling = false;

        this.handleScroll = (e) => {
            if (this.isScrolling) return;

            const delta = Math.sign(e.deltaY);

            if (delta > 0 && this.currentSection < this.sections.length - 1) {
                e.preventDefault();
                this.scrollToSection(this.currentSection + 1);
            }
        };

        window.addEventListener("wheel", this.handleScroll, { passive: false });

        // Detect current visible section on load
        this.updateCurrentSection();
        window.addEventListener("scroll", this.updateCurrentSection);
    },
    beforeUnmount() {
        window.removeEventListener("wheel", this.handleScroll);
        window.removeEventListener("scroll", this.updateCurrentSection);
    },
};
</script>

<style scoped>
/* Custom navigation buttons */
.mySwiper .swiper-button-next,
.mySwiper .swiper-button-prev {
    color: #ffffff;
    background: #547326;
    border-radius: 5px;
    width: 36px;
    height: 28px;
    margin-top: -25px;
    top: 90%;
    transition: all 0.3s ease-in-out;
}

.mySwiper .swiper-button-next:hover,
.mySwiper .swiper-button-prev:hover {
    background-color: #ffffff;
    color: #547326;
}

.mySwiper .swiper-button-prev {
    left: 90% !important;
}

.mySwiper .swiper-button-next {
    left: 93% !important;
}

.mySwiper .swiper-button-next:after,
.mySwiper .swiper-button-prev:after {
    font-size: 18px;
    font-weight: bold;
}

/* Custom pagination */
.mySwiper .swiper-pagination {
    bottom: 20px;
}

.mySwiper .swiper-pagination-bullet {
    width: 12px;
    height: 12px;
    background: rgba(255, 255, 255, 0.5);
    opacity: 1;
}

.mySwiper .swiper-pagination-bullet-active {
    background: #ffffff;
}

/* Ensure slides don't stack */
.mySwiper .swiper-wrapper {
    display: flex;
    transition-property: transform;
}

.mySwiper .swiper-slide {
    flex-shrink: 0;
    width: 100%;
    height: 100%;
    position: relative;
}
</style>
