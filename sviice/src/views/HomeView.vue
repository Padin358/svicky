<script setup>
import HeadSec from '@/components/sections/HeadSec.vue';
import MainSec from "@/components/sections/MainSec.vue";
import ScrollIndicator from "@/components/ScrollIndicator.vue";
import Sec1 from "@/components/sections/subSections/Sec1.vue";
import Sec2 from "@/components/sections/subSections/Sec2.vue";
import Sec3 from "@/components/sections/subSections/Sec3.vue";
import Sec4 from "@/components/sections/subSections/Sec4.vue";
import FootSec from "@/components/sections/FootSec.vue";
</script>

<template>
  <ScrollIndicator />
  <HeadSec page="HomeView"/>
  <MainSec />
  <Sec1/>
  <hr class="text-[#dfdfdf]/50 mt-16 mx-24">
  <Sec2/>
  <hr class="text-[#dfdfdf]/50 mt-16 mx-24">
  <Sec3/>
  <hr class="text-[#dfdfdf]/50 mt-16 mx-24">
  <Sec4/>
  <div class="h-70"></div>
</template>
