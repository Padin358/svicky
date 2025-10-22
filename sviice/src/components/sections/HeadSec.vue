<template>
  <div class="mt-16 h-50 xl:h-100 w-full bg-[url(@/assets/img/banner.png)] bg-cover bg-center transition-all duration-500 z-0 flex flex-col justify-center items-center" v-html="content">

  </div>
</template>

<script setup>
import {ref, defineProps} from "vue";

const props = defineProps({
  page: String,
})

let content = ref("")

setTimeout(() => {
  switch (props.page) {
    case 'HomeView':
      content.value = "<p class='text-3xl lg:text-6xl bg-linear-to-r from-white to-yellow-200 bg-clip-text text-transparent z-10 font-black transition-all duration-500'>SmartCandles</p><p class='text:lg lg:text-xl text-gray-50 font-semibold'>První svíčky, co myslí s vámi...</p>"
      break
    case 'FaqView':
      break
    case 'ProductsView':
      break
    default:
      break
  }
}, 1000)

</script>