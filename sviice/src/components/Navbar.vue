<template>
  <div class="fixed top-0 left-0 w-full p-5 bg-black/97 flex flex-row flex-wrap justify-between text-[#dfdfdf] text-md md:text-xl font-medium z-30 items-center">
    <RouterLink to="/" class="hidden md:flex justify-center gap-0 items-center hover:opacity-75 transition-all duration-300"><img src="@/assets/img/logo_white_small.png" alt="" class="w-10 h-10">SmartCandles</RouterLink>
    <div class="flex flex-row flex-wrap justify-end gap-3 md:gap-10 items-center">
      <RouterLink to="/" class="after:block after:border-b-3 after:border-b-[#dfdfdf] after:scale-x-0 hover:after:scale-x-100 after:origin-bottom-left after:transition-all after:duration-150">Úvod</RouterLink>
      <RouterLink to="/products/" class="after:block after:border-b-3 after:border-b-[#dfdfdf] after:scale-x-0 hover:after:scale-x-100 after:origin-bottom-left after:transition-all after:duration-150">Produkty</RouterLink>
      <RouterLink to="/faq/" class="after:block after:border-b-3 after:border-b-[#dfdfdf] after:scale-x-0 hover:after:scale-x-100 after:origin-bottom-left after:transition-all after:duration-150">FAQ</RouterLink>
    </div>
  </div>
</template>

<script setup>
import { RouterLink } from 'vue-router';

</script>