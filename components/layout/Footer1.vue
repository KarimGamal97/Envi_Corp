<template>
    <footer class="bg-[#08223B]">
        <div class="px-10 md:px-40">
            <div
                class="text-white grid gird-cols-1 gap-8 md:grid-cols-2 lg:grid-cols-5 xl:gap-[98px] py-20 md:py-40"
            >
                <div class="lg:col-span-2 flex flex-col gap-5">
                    <img
                        src="/assets/images/main-imgs/main-logo-light.png"
                        class="logo z-50 w-[40%] mb-5"
                        alt="logo"
                    />
                    <p class="mb-3 text-clamp">
                        Subscribe to our newsletter for the latest updates on features and releases.
                    </p>
                    <form class="flex gap-2 w-full">
                        <input
                            type="email"
                            placeholder="Enter your email"
                            class="flex-1 rounded p-3"
                        />
                        <button
                            type="submit"
                            class="bg-white text-black rounded py-2 px-4 hover:bg-[#547326] hover:text-white transition-all duration-200"
                        >
                            Join
                        </button>
                    </form>
                    <p class="text-md">
                        By subscribing, you consent to our Privacy Policy and receiving updates.
                    </p>
                </div>
                <div>
                    <h5 class="text-heading-4 font-poppins mb-10">Quick Links</h5>
                    <ul>
                        <li class="mb-5">
                            <a
                                class="text-clamp transition-all duration-200 hover:text-green-900 hover:pl-[3px]"
                                href="#"
                                >About Us</a
                            >
                        </li>
                        <li class="mb-5">
                            <a
                                class="text-clamp transition-all duration-200 hover:text-green-900 hover:pl-[3px]"
                                href="#"
                                >Services</a
                            >
                        </li>
                        <li class="mb-5">
                            <a
                                class="text-clamp transition-all duration-200 hover:text-green-900 hover:pl-[3px]"
                                href="#"
                                >Contact Us</a
                            >
                        </li>
                        <li class="mb-5">
                            <a
                                class="text-clamp transition-all duration-200 hover:text-green-900 hover:pl-[3px]"
                                href="#"
                                >Blog</a
                            >
                        </li>
                        <li class="mb-5">
                            <a
                                class="text-clamp transition-all duration-200 hover:text-green-900 hover:pl-[3px]"
                                href="#"
                                >Careers</a
                            >
                        </li>
                    </ul>
                </div>
                <div>
                    <h5 class="text-heading-4 font-poppins mb-10 text-[18px]">Resources</h5>
                    <ul>
                        <li class="mb-5">
                            <a
                                class="text-clamp transition-all duration-200 hover:text-green-900 hover:pl-[3px]"
                                href="/faqs"
                                >FAQs</a
                            >
                        </li>
                        <li class="mb-5">
                            <a
                                class="text-clamp transition-all duration-200 hover:text-green-900 hover:pl-[3px]"
                                href="/terms-conditions"
                                >Case Studies</a
                            >
                        </li>
                        <li class="mb-5">
                            <a
                                class="text-clamp transition-all duration-200 hover:text-green-900 hover:pl-[3px]"
                                href="/privacy-policy"
                                >White Papers</a
                            >
                        </li>
                        <li class="mb-5">
                            <a
                                class="text-clamp transition-all duration-200 hover:text-green-900 hover:pl-[3px]"
                                href="/contact"
                                >Webinars</a
                            >
                        </li>
                        <li class="mb-5">
                            <a
                                class="text-clamp transition-all duration-200 hover:text-green-900 hover:pl-[3px]"
                                href="/contact"
                                >Careers</a
                            >
                        </li>
                    </ul>
                </div>
                <div>
                    <h5 class="text-heading-4 font-poppins mb-10 text-[18px]">Connect With Us</h5>
                    <ul>
                        <li class="mb-5">
                            <NuxtLink class="flex items-center gap-3" to="#">
                                <img src="/assets/images/icons/facebook.svg" alt="" />
                                <span class="text-clamp">Facebook</span>
                            </NuxtLink>
                        </li>
                        <li class="mb-5">
                            <NuxtLink class="flex items-center gap-3" to="#">
                                <img src="/assets/images/icons/insta.svg" alt="" />
                                <span class="text-clamp">Instagram</span>
                            </NuxtLink>
                        </li>
                        <li class="mb-5">
                            <NuxtLink class="flex items-center gap-3" to="#">
                                <img src="/assets/images/icons/X.svg" alt="" />
                                <span class="text-clamp">Twitter</span>
                            </NuxtLink>
                        </li>
                        <li class="mb-5">
                            <NuxtLink class="flex items-center gap-3" to="#">
                                <img src="/assets/images/icons/linkedin.svg" alt="" />
                                <span class="text-clamp">Linkedin</span>
                            </NuxtLink>
                        </li>
                        <li class="mb-5">
                            <NuxtLink class="flex items-center gap-3" to="#">
                                <img src="/assets/images/icons/youtube.svg" alt="" />
                                <span class="text-clamp">Youtube</span>
                            </NuxtLink>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
        <div
            class="bg-[#547326] text-black lg:flex lg:items-center lg:justify-between px-[12px] md:px-[36px] py-2"
        >
            <div class="md:flex md:items-center md:gap-6">
                <p class="text-clamp">© 2025 Envi-comm. All rights reserved.</p>
            </div>
            <div class="flex items-center justify-between md:gap-6">
                <a class="underline text-clamp" href="#">Privacy Policy</a
                ><a class="underline text-clamp" href="#">Terms of Use</a
                ><a class="underline text-clamp" href="#">Cookie Settings</a>
            </div>
        </div>
    </footer>
</template>
