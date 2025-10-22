<template>
  <div class="">
    <Navbar />
    <RouterView />
    <FootSec/>
  </div>
</template>

<script setup>
import Navbar from '@/components/Navbar.vue';
import { RouterView } from 'vue-router';
import FootSec from "@/components/sections/FootSec.vue";
import HeadSec from "@/components/sections/HeadSec.vue";
</script>