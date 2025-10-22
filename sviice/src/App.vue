<template>
  <div class="">
    <Navbar />
    <RouterView />
  </div>
</template>

<script setup>
import Navbar from '@/components/Navbar.vue';
import { RouterView } from 'vue-router';
</script>