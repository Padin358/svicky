<script setup>
import HeadSec from '@/components/sections/HeadSec.vue';
import HomeMainSec from "@/components/sections/HomeMainSec.vue";
import ScrollIndicator from "@/components/ScrollIndicator.vue";
</script>

<template>
  <ScrollIndicator />
  <HeadSec page="HomeView"/>
  <HomeMainSec />
  <div class="h-70"></div>
</template>
