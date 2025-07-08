<template>
    <section id="section1" class="w-full min-h-dvh md:h-screen">
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
            class="mySwiper min-h-dvh md:h-screen w-full relative overflow-hidden"
        >
            <!-- Slide 1 -->
            <SwiperSlide class="min-h-dvh md:h-screen w-full">
                <div
                    class="relative w-full min-h-dvh md:h-screen bg-cover bg-left md:bg-center bg-no-repeat bg-[url('/assets/images/main-imgs/slider-01.jpg')]"
                >
                    <div
                        class="relative z-10 p-8 flex flex-col justify-center min-h-dvh md:h-screen"
                    >
                        <h2 class="text-3xl md:text-5xl mb-10 text-black md:max-w-[35%]">
                            STP & WTP SYSTEMS Engineered for Efficiency
                        </h2>
                        <p class="text-xl text-black mb-10 md:max-w-[25%]">
                            One-stop solutions for effective wastewater and water treatment with
                            minimal downtime and maximum performance.
                        </p>
                        <button class="bg-[#547326] rounded-md text-white px-5 py-2 w-fit">
                            Know More
                        </button>
                    </div>
                </div>
            </SwiperSlide>

            <!-- Slide 2 -->
            <SwiperSlide class="min-h-dvh md:h-screen w-full">
                <div
                    class="relative w-full min-h-dvh md:h-screen bg-cover bg-left md:bg-center bg-no-repeat bg-[url('/assets/images/main-imgs/slider-02.jpg')]"
                >
                    <div
                        class="relative z-10 p-8 flex flex-col justify-center min-h-dvh md:h-screen"
                    >
                        <h2 class="text-3xl md:text-5xl mb-10 text-white md:max-w-[35%]">
                            EIS Tailored for Your Industry
                        </h2>
                        <p class="text-xl text-white mb-10 md:max-w-[25%]">
                            Whether infrastructure, energy, or development — our Environmental
                            Impact Studies are built to match your sector's needs.
                        </p>
                        <button class="bg-[#547326] rounded-md text-white px-5 py-2 w-fit">
                            Know More
                        </button>
                    </div>
                </div>
            </SwiperSlide>

            <!-- Slide 3 -->
            <SwiperSlide class="min-h-dvh md:h-screen w-full">
                <div
                    class="relative w-full min-h-dvh md:h-screen bg-cover bg-left md:bg-center bg-no-repeat bg-[url('/assets/images/main-imgs/slider-03.jpg')]"
                >
                    <div
                        class="relative z-10 p-8 flex flex-col justify-center min-h-dvh md:h-screen"
                    >
                        <h2 class="text-3xl md:text-5xl mb-10 text-black md:max-w-[35%]">
                            Solar Streetlight That Saves More Than Just Power
                        </h2>
                        <p class="text-xl text-black mb-10 md:max-w-[25%]">
                            Introducing our 150W Solar Streetlight Harness the sun to save
                            electricity, cut carbon emissions, and protect the planet — without
                            compromising brightness or reliability.
                        </p>
                        <button class="bg-[#547326] rounded-md text-white px-5 py-2 w-fit">
                            Know More
                        </button>
                    </div>
                </div>
            </SwiperSlide>

            <!-- Slide 4 -->
            <SwiperSlide class="min-h-dvh md:h-screen w-full">
                <div
                    class="relative w-full min-h-dvh md:h-screen bg-cover bg-left md:bg-center bg-no-repeat bg-[url('/assets/images/main-imgs/slider-04.jpg')]"
                >
                    <div
                        class="relative z-10 p-8 flex flex-col justify-center min-h-dvh md:h-screen"
                    >
                        <h2 class="text-3xl md:text-5xl mb-10 text-white md:max-w-[35%]">
                            Secure Your DENR Certificate of Tree Planting
                        </h2>
                        <button
                            class="bg-transparent border-2 border-white rounded-md text-white px-5 py-2 w-fit"
                        >
                            Know More
                        </button>
                    </div>
                </div>
            </SwiperSlide>

            <!-- Slide 5 -->
            <SwiperSlide class="min-h-dvh md:h-screen w-full">
                <div
                    class="relative w-full min-h-dvh md:h-screen bg-cover bg-left md:bg-center bg-no-repeat bg-[url('/assets/images/main-imgs/slider-05.jpg')]"
                >
                    <div
                        class="relative z-10 p-8 flex flex-col justify-center min-h-dvh md:h-screen"
                    >
                        <h2 class="text-3xl md:text-5xl mb-10 text-black md:max-w-[35%]">
                            Compliance Made Simple. Savings Made Easy.
                        </h2>
                        <p class="text-xl text-black mb-10 md:max-w-[25%]">
                            Envi-comm’s Retainership Program gives you continuous support and peace
                            of mind, so you can run your business worry-free.
                        </p>
                        <button class="bg-[#547326] rounded-md text-white px-5 py-2 w-fit">
                            Know More
                        </button>
                    </div>
                </div>
            </SwiperSlide>

            <!-- Slide 6 -->
            <SwiperSlide class="min-h-dvh md:h-screen w-full">
                <div
                    class="relative w-full min-h-dvh md:h-screen bg-cover bg-left md:bg-center bg-no-repeat bg-[url('/assets/images/main-imgs/slider-06.jpg')]"
                >
                    <div
                        class="relative z-10 p-8 flex flex-col justify-center min-h-dvh md:h-screen"
                    >
                        <h2 class="text-3xl md:text-5xl mb-5 text-black md:max-w-[35%]">
                            Clean Water Starts with Proven Chemistry
                        </h2>
                        <p class="text-xl text-black mb-5 md:max-w-[25%]">
                            Envi-comm Corporation provides high-performance chemical solutions
                            tailored for optimal sludge control, odor management, and regulatory
                            compliance.
                        </p>
                        <button class="bg-[#547326] rounded-md text-white px-5 py-2 w-fit">
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
        <div
            class="flex flex-col md:flex-row justify-between gap-3 bg-[#1C1C1C] px-10 md:px-20 py-3"
        >
            <button
                v-for="(title, index) in slideTitles"
                :key="index"
                @click="goToSlide(index)"
                :class="[
                    'text-md transition-all duration-200 uppercase',
                    currentSlideIndex === index ? 'font-semibold text-white' : 'text-gray-200',
                ]"
            >
                {{ title }}
            </button>
        </div>
    </section>

    <!-- <section id="section2">
        <div class="px-[12px] md:px-[36px] xl:px-0 mt-[70px] lg:mt-[150px]">
            <span
                class="font-chivo inline-block bg-bg-2 text-green-900 py-[14px] px-[28px] rounded-[50px] text-[14px] leading-[14px] mb-8"
                >Company Overview</span
            >
            <div class="mb-14">
                <h2
                    class="text-gray-900 font-bold font-chivo mb-5 text-[35px] leading-[44px] md:text-[46px] md:leading-[52px] lg:text-heading-1 md:mb-[30px] max-w-[725px]"
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
                            class="min-h-dvh md:h-screen w-full object-cover rounded-2xl mb-[30px]"
                            src="/assets/images/destination-1.png"
                            alt="Img"
                        />
                    </div>
                    <div class="flex items-center gap-[10px] mb-[11px]"></div>
                    <h4
                        class="font-bold font-chivo text-[14px] xl:text-heading-5 mb-[15px] text-center"
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
                            class="min-h-dvh md:h-screen w-full object-cover rounded-2xl mb-[30px]"
                            src="/assets/images/destination-1.png"
                            alt="Img"
                        />
                    </div>
                    <div class="flex items-center gap-[10px] mb-[11px]"></div>
                    <h4
                        class="font-bold font-chivo text-[14px] xl:text-heading-5 mb-[15px] text-center"
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
                        class="font-bold font-chivo text-[14px] xl:text-heading-5 mb-[15px] text-center"
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
                        class="block text-inherit w-full h-full rounded-[50px] text-lg font-chivo font-semibold"
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
    <section id="section3">
        <div class="px-5 md:px-20 mt-20 md:mt-[150px]">
            <h2
                class="text-center text-gray-900 uppercase font-chivo mb-5 text-[35px] leading-[44px] md:text-[46px] lg:text-heading-1 md:mb-[30px]"
            >
                What We Do
            </h2>
            <div class="grid grid-cols-1 md:grid-cols-2 xl:grid-cols-3 gap-5 mb-[52px]">
                <!-- items 1 -->
                <div class="relative rounded-lg overflow-hidden h-[180px] group">
                    <div class="absolute inset-0 bg-black/40 w-full h-full"></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_01.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3 class="text-white underline text-2xl absolute bottom-10 left-10">
                        Planning
                    </h3>
                </div>
                <!-- items 2 -->
                <div class="relative rounded-lg overflow-hidden h-[180px] group">
                    <div class="absolute inset-0 bg-black/40 w-full h-full"></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_02.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3 class="text-white underline text-2xl absolute bottom-10 left-10">
                        Permitting
                    </h3>
                </div>
                <!-- items 3 -->
                <div class="relative rounded-lg overflow-hidden h-[180px] group">
                    <div class="absolute inset-0 bg-black/40 w-full h-full"></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_03.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3 class="text-white underline text-2xl absolute bottom-10 left-10">
                        Reporting
                    </h3>
                </div>
                <!-- items 4 -->
                <div class="relative rounded-lg overflow-hidden h-[180px] group">
                    <div class="absolute inset-0 bg-black/40 w-full h-full"></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_04.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3 class="text-white underline text-2xl absolute bottom-10 left-10">STPs</h3>
                </div>
                <!-- items 5 -->
                <div class="relative rounded-lg overflow-hidden h-[180px] group">
                    <div class="absolute inset-0 bg-black/40 w-full h-full"></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_05.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3 class="text-white underline text-2xl absolute bottom-10 left-10">
                        STP Chemicals
                    </h3>
                </div>
                <!-- items 6 -->
                <div class="relative rounded-lg overflow-hidden h-[180px] group">
                    <div class="absolute inset-0 bg-black/40 w-full h-full"></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_06.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3 class="text-white underline text-2xl absolute bottom-10 left-10">Solar</h3>
                </div>
                <!-- items 7 -->
                <div class="relative rounded-lg overflow-hidden h-[180px] group">
                    <div class="absolute inset-0 bg-black/40 w-full h-full"></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_07.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3 class="text-white underline text-2xl absolute bottom-10 left-10">
                        Hauling & Septage
                    </h3>
                </div>
                <!-- items 8 -->
                <div class="relative rounded-lg overflow-hidden h-[180px] group">
                    <div class="absolute inset-0 bg-black/40 w-full h-full"></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_08.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3 class="text-white underline text-2xl absolute bottom-10 left-10">Saas</h3>
                </div>
                <!-- items 9 -->
                <div class="relative rounded-lg overflow-hidden h-[180px] group">
                    <div class="absolute inset-0 bg-black/40 w-full h-full"></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_09.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3 class="text-white underline text-2xl absolute bottom-10 left-10">
                        Training
                    </h3>
                </div>
                <!-- items 10 -->
                <div class="relative rounded-lg overflow-hidden h-[180px] group">
                    <div class="absolute inset-0 bg-black/40 w-full h-full"></div>
                    <img
                        src="/assets/images/main-imgs/what_we_do_10.jpg"
                        alt="planning"
                        class="absolute inset-0 z-[-1] w-full h-full object-cover object-center group-hover:scale-110 transition-all duration-300"
                        loading="lazy"
                    />
                    <h3 class="text-white underline text-2xl absolute bottom-10 left-10">
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
                "Get STP & WTP Solutions",
                "Begin EIS Process",
                "Go Solar Today",
                "Avail Tree Planting Certificate",
                "Claim Your Retainership Plan",
                "Request Custom Chemical Solutions",
            ],
            modules: [Navigation, Pagination, Autoplay],
        };
    },
    methods: {
        onSwiper(swiper) {
            this.swiperInstance = swiper;

            // بنسجل تغيير السلايد عشان نعمل active للزر
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
    },
    mounted() {
        this.$nextTick(() => {
            this.swiperInstance = this.$refs.mySwiper.swiper;
        });
        // Define the scroll handler function
        //         this.handleScroll = (event) => {
        //             if (this.isScrolling) return;
        //             // Check if the scroll event is happening within the Swiper area
        //             const swiperElement = event.target.closest(".mySwiper");
        //             if (swiperElement) {
        //                 return; // Don't handle scroll if it's within the Swiper
        //             }
        //             const delta = Math.sign(event.deltaY);
        //             if (delta > 0 && this.currentSection < this.sections.length - 1) {
        //                 // Scroll down
        //                 this.scrollToSection(this.currentSection + 1);
        //             } else if (delta < 0 && this.currentSection > 0) {
        //                 // Scroll up
        //                 this.scrollToSection(this.currentSection - 1);
        //             }
        //         };
        //         // Initialize variables
        //         this.sections = document.querySelectorAll("section");
        //         this.currentSection = 0;
        //         this.isScrolling = false;
        //         // Add event listener
        //         window.addEventListener("wheel", this.handleScroll);
        //         // Set initial section as active
        //         const initialSection = document.getElementById("section1");
        //         if (initialSection) {
        //             initialSection.classList.add("active");
        //         }
        //     },
        //     beforeUnmount() {
        //         // Remove the event listener when the component is destroyed
        //         window.removeEventListener("wheel", this.handleScroll);
        //     },
        //     methods: {
        //         scrollToSection(index) {
        //             this.isScrolling = true;
        //             const targetSection = this.sections[index];
        //             const targetPosition = targetSection.offsetTop;
        //             const startPosition = window.pageYOffset;
        //             const distance = targetPosition - startPosition;
        //             const duration = 1000;
        //             let startTimestamp = null;
        //             const scrollStep = (timestamp) => {
        //                 if (!startTimestamp) startTimestamp = timestamp;
        //                 const progress = timestamp - startTimestamp;
        //                 window.scrollTo(
        //                     0,
        //                     this.easeInOutCubic(progress, startPosition, distance, duration)
        //                 );
        //                 if (progress < duration) {
        //                     window.requestAnimationFrame(scrollStep);
        //                 } else {
        //                     this.currentSection = index;
        //                     this.isScrolling = false;
        //                     window.scrollTo(0, targetPosition);
        //                 }
        //             };
        //             window.requestAnimationFrame(scrollStep);
        //         },
        //         easeInOutCubic(t, b, c, d) {
        //             t /= d / 2;
        //             if (t < 1) return (c / 2) * t * t * t + b;
        //             t -= 2;
        //             return (c / 2) * (t * t * t + 2) + b;
        //         },
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
