<template>
  <section id="section1">
    <Swiper
      :modules="modules"
      :slides-per-view="1"
      :space-between="0"
      :loop="true"
      :pagination="{
        clickable: true,
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
      class="mySwiper"
    >
      <SwiperSlide v-for="(slide, index) in slides" :key="index">
        <div class="px-[12px] grid lg:mt-[90px]">
          <div
            class="flex-1 relative"
            :style="{
              backgroundImage: `url('${slide.image}')`,
              backgroundSize: 'cover',
              backgroundPosition: 'center',
              backgroundRepeat: 'no-repeat',
              height: '70vh',
            }"
          >
            <div class="absolute inset-0 bg-black bg-opacity-30"></div>
            <div
              class="relative z-10 p-8 flex flex-col justify-center h-full"
              style="width: 1080px"
            >
              <p
                class="text-gray-600 mb-[45px] max-w-[50%]"
                style="font-size: 2.5rem; line-height: 1.3; margin-top: 50px"
              >
                {{ slide.title }}
              </p>
              <button
                class="bg-green-900 text-white px-5 py-2 w-fit hidden"
                style="border-radius: 6px"
              >
                {{ slide.buttonText }}
              </button>
            </div>
          </div>
        </div>
      </SwiperSlide>

      <!-- Navigation buttons -->
      <div class="swiper-button-next"></div>
      <div class="swiper-button-prev"></div>

      <!-- Pagination -->
      <div class="swiper-pagination"></div>
    </Swiper>
  </section>
  <section id="section2">
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
          We are a team of environmental experts dedicated to assisting
          businesses.
        </p>
      </div>
      <div
        class="grid grid-cols-1 md:grid-cols-2 xl:grid-cols-3 gap-x-[30px] gap-y-[50px] mb-[52px]"
      >
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
            Streamlining the environmental application process for our clients
            to ensure compliance and expedite project approvals.
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
            Streamlining the environmental application process for our clients
            to ensure compliance and expedite project approvals.
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
            Streamlining the environmental application process for our clients
            to ensure compliance and expedite project approvals.
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
  </section>
  <section id="section3">
    <div class="px-[12px] md:px-[36px] xl:px-0 mt-[70px] lg:mt-[150px]">
      <h2
        class="text-center text-gray-900 font-bold font-chivo mb-5 text-[35px] leading-[44px] md:text-[46px] md:leading-[52px] lg:text-heading-1 md:mb-[30px]"
      >
        What We Do
      </h2>
      <div
        class="grid grid-cols-1 md:grid-cols-2 xl:grid-cols-3 gap-x-[30px] gap-y-[50px] mb-[52px]"
      >
        <div>
          <p
            style="
              background-image: url('/assets/images/main-imgs/what_we_do_01.jpg');
              background-position: center;
              background-repeat: no-repeat;
              background-size: cover;
              color: white;
              font-size: 24px;
              font-weight: bold;
              height: 150px;
              filter: brightness(0.8);
              border-radius: 6px;
            "
          >
            Planning
          </p>
        </div>
        <div>
          <p
            style="
              background-image: url('/assets/images/main-imgs/what_we_do_02.jpg');
              background-position: center;
              background-repeat: no-repeat;
              background-size: cover;
              color: white;
              font-size: 24px;
              font-weight: bold;
              height: 150px;
              filter: brightness(0.8);
              border-radius: 6px;
            "
          >
            Permitting
          </p>
        </div>
        <div>
          <p
            style="
              background-image: url('/assets/images/main-imgs/what_we_do_03.jpg');
              background-position: center;
              background-repeat: no-repeat;
              background-size: cover;
              color: white;
              font-size: 24px;
              font-weight: bold;
              height: 150px;
              filter: brightness(0.8);
              border-radius: 6px;
            "
          >
            Reporting
          </p>
        </div>
        <div>
          <p
            style="
              background-image: url('/assets/images/main-imgs/what_we_do_04.jpg');
              background-position: center;
              background-repeat: no-repeat;
              background-size: cover;
              color: white;
              font-size: 24px;
              font-weight: bold;
              height: 150px;
              filter: brightness(0.8);
              border-radius: 6px;
            "
          >
            STPs
          </p>
        </div>
        <div>
          <p
            style="
              background-image: url('/assets/images/main-imgs/what_we_do_05.jpg');
              background-position: center;
              background-repeat: no-repeat;
              background-size: cover;
              color: white;
              font-size: 24px;
              font-weight: bold;
              height: 150px;
              filter: brightness(0.8);
              border-radius: 6px;
            "
          >
            STP Chemicals
          </p>
        </div>
        <div>
          <p
            style="
              background-image: url('/assets/images/main-imgs/what_we_do_06.jpg');
              background-position: center;
              background-repeat: no-repeat;
              background-size: cover;
              color: white;
              font-size: 24px;
              font-weight: bold;
              height: 150px;
              filter: brightness(0.8);
              border-radius: 6px;
            "
          >
            Solar
          </p>
        </div>
        <div>
          <p
            style="
              background-image: url('/assets/images/main-imgs/what_we_do_07.jpg');
              background-position: center;
              background-repeat: no-repeat;
              background-size: cover;
              color: white;
              font-size: 24px;
              font-weight: bold;
              height: 150px;
              filter: brightness(0.8);
              border-radius: 6px;
            "
          >
            Hauling & Septage
          </p>
        </div>
        <div>
          <p
            style="
              background-image: url('/assets/images/main-imgs/what_we_do_08.jpg');
              background-position: center;
              background-repeat: no-repeat;
              background-size: cover;
              color: white;
              font-size: 24px;
              font-weight: bold;
              height: 150px;
              filter: brightness(0.8);
              border-radius: 6px;
            "
          >
            Saas
          </p>
        </div>
        <div>
          <p
            style="
              background-image: url('/assets/images/main-imgs/what_we_do_09.jpg');
              background-position: center;
              background-repeat: no-repeat;
              background-size: cover;
              color: white;
              font-size: 24px;
              font-weight: bold;
              height: 150px;
              filter: brightness(0.8);
              border-radius: 6px;
            "
          >
            Training
          </p>
        </div>
        <div>
          <p
            style="
              background-image: url('/assets/images/main-imgs/what_we_do_10.jpg');
              background-position: center;
              background-repeat: no-repeat;
              background-size: cover;
              color: white;
              font-size: 24px;
              font-weight: bold;
              height: 150px;
              filter: brightness(0.8);
              border-radius: 6px;
            "
          >
            Planning
          </p>
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
      modules: [Navigation, Pagination, Autoplay],
      slides: [
        {
          image: "/assets/images/main-imgs/slider-01.jpg",
          title:
            "We are your trusted experts in environmental impact study (EIS) preparation",
          buttonText: "Know More",
        },
        {
          image: "/assets/images/main-imgs/slider-02.jpg",
          // title:
          //   "Comprehensive environmental consulting services for sustainable development",
          // buttonText: "Learn More",
        },
        {
          image: "/assets/images/main-imgs/slider-03.jpg",
          // title:
          //   "Expert guidance for environmental compliance and regulatory requirements",
          // buttonText: "Discover More",
        },
      ],
    };
  },
  mounted() {
    // Define the scroll handler function
    this.handleScroll = (event) => {
      if (this.isScrolling) return;

      // Check if the scroll event is happening within the Swiper area
      const swiperElement = event.target.closest(".mySwiper");
      if (swiperElement) {
        return; // Don't handle scroll if it's within the Swiper
      }

      const delta = Math.sign(event.deltaY);

      if (delta > 0 && this.currentSection < this.sections.length - 1) {
        // Scroll down
        this.scrollToSection(this.currentSection + 1);
      } else if (delta < 0 && this.currentSection > 0) {
        // Scroll up
        this.scrollToSection(this.currentSection - 1);
      }
    };

    // Initialize variables
    this.sections = document.querySelectorAll("section");
    this.currentSection = 0;
    this.isScrolling = false;

    // Add event listener
    window.addEventListener("wheel", this.handleScroll);

    // Set initial section as active
    const initialSection = document.getElementById("section1");
    if (initialSection) {
      initialSection.classList.add("active");
    }
  },
  beforeUnmount() {
    // Remove the event listener when the component is destroyed
    window.removeEventListener("wheel", this.handleScroll);
  },
  methods: {
    scrollToSection(index) {
      this.isScrolling = true;
      const targetSection = this.sections[index];
      const targetPosition = targetSection.offsetTop;
      const startPosition = window.pageYOffset;
      const distance = targetPosition - startPosition;
      const duration = 1000;
      let startTimestamp = null;

      const scrollStep = (timestamp) => {
        if (!startTimestamp) startTimestamp = timestamp;
        const progress = timestamp - startTimestamp;

        window.scrollTo(
          0,
          this.easeInOutCubic(progress, startPosition, distance, duration)
        );

        if (progress < duration) {
          window.requestAnimationFrame(scrollStep);
        } else {
          this.currentSection = index;
          this.isScrolling = false;
          window.scrollTo(0, targetPosition);
        }
      };

      window.requestAnimationFrame(scrollStep);
    },
    easeInOutCubic(t, b, c, d) {
      t /= d / 2;
      if (t < 1) return (c / 2) * t * t * t + b;
      t -= 2;
      return (c / 2) * (t * t * t + 2) + b;
    },
  },
};
</script>

<style scoped>
.mySwiper {
  width: 100%;
  height: 100%;
}

/* Custom navigation buttons */
.mySwiper .swiper-button-next,
.mySwiper .swiper-button-prev {
  color: #ffffff;
  background: rgba(0, 0, 0, 0.5);
  border-radius: 50%;
  width: 50px;
  height: 50px;
  margin-top: -25px;
}

.mySwiper .swiper-button-next:after,
.mySwiper .swiper-button-prev:after {
  font-size: 18px;
  font-weight: bold;
}

.mySwiper .swiper-button-next:hover,
.mySwiper .swiper-button-prev:hover {
  background: rgba(0, 0, 0, 0.8);
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
