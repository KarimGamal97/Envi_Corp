<template>
  <LayoutTopbar1 />
  <div class="wrapper mx-auto text-gray-900 font-normal max-w-[1320px]">
    <LayoutHeader1 />
    <div>
      <slot />
    </div>
    <ElementsBackToTop />
    <ElementsInquiryBtn />
    <LayoutFooter1 />
  </div>
</template>
