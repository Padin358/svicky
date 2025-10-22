<template>
  <div class="fixed top-0 left-0 w-full p-5 bg-gray-950 flex flex-row flex-wrap justify-between text-[#dfdfdf] text-xl font-medium">
    <div class="">Jakože logo, ok?</div>
    <div class="flex flex-row flex-wrap justify-end gap-3">
      <RouterLink to="/" class="after:block after:border-b-2 after:border-b-[#dfdfdf] after:scale-x-0 hover:after:scale-x-100 after:origin-bottom-left after:transition-all after:duration-200">Úvod</RouterLink>
      <RouterLink to="/products/" class="after:block after:border-b-2 after:border-b-[#dfdfdf] after:scale-x-0 hover:after:scale-x-100 after:origin-bottom-left after:transition-all after:duration-200">Produkty</RouterLink>
      <RouterLink to="/contacts/" class="after:block after:border-b-2 after:border-b-[#dfdfdf] after:scale-x-0 hover:after:scale-x-100 after:origin-bottom-left after:transition-all after:duration-200">Kontakt</RouterLink>
      <RouterLink to="/faq/" class="after:block after:border-b-2 after:border-b-[#dfdfdf] after:scale-x-0 hover:after:scale-x-100 after:origin-bottom-left after:transition-all after:duration-200">FAQ</RouterLink>
    </div>
  </div>
</template>

<script setup>
import { RouterLink } from 'vue-router';

</script>