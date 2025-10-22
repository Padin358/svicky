<template>
  <div class="hidden fixed right-5 top-1/2 -translate-y-1/2 z-20 text-md font-semibold text-white lg:flex flex-col justify-center text-right gap-2">
    <a
        v-for="section in sections"
        :key="section.id"
        :href="`#${section.id}`"
        class="after:content-['•'] after:ml-2 transition-all duration-300 hover:text-white/50"
    >
      {{section.name}}
    </a>
  </div>
</template>

<script setup>

const sections = [
  {name: "Úvod", id: 1},
  {name: "Historie", id: 2},
  {name: "AI", id: 3},
  {name: "Tým", id: 4},
]

</script>