<template>
  <div className='w-full h-12 bg-linear-to-b from-black/80 to-black/0'></div>
  <Sec1/>
  <hr class="text-[#dfdfdf]/50 mt-16 mx-24">
  <Sec2/>
  <hr class="text-[#dfdfdf]/50 mt-16 mx-24">
  <Sec3/>
  <hr class="text-[#dfdfdf]/50 mt-16 mx-24">
  <Sec4/>
</template>

<script setup>

import Sec2 from "@/components/sections/subSections/Sec2.vue";
import Sec1 from "@/components/sections/subSections/Sec1.vue";
import Sec3 from "@/components/sections/subSections/Sec3.vue";
import Sec4 from "@/components/sections/subSections/Sec4.vue";
</script>