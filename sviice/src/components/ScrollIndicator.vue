<template>
  <div class="fixed right-5 top-1/2 -translate-y-1/2 z-20 text-md font-semibold text-white flex flex-col justify-center text-right gap-2">
    <a
        v-for="section in sections"
        :key="section.id"
        :href="`#${section.id}`"
        @click.prevent="scrollToSection(section.id)"
        class="after:content-['•'] after:ml-2 transition-all duration-300"
        :class="activeSection === section.id ? 'text-yellow-300 scale-110' : 'text-white hover:text-gray-300'"
    >
      {{section.name}}
    </a>
  </div>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from 'vue';

const sections = [
  {name: "Úvod", id: 1},
  {name: "Historie", id: 2},
  {name: "AI", id: 3},
  {name: "Tým", id: 4},
]

const activeSection = ref(1);

const handleScroll = () => {
  const scrollPosition = window.scrollY + 100;

  // Zjisti, jestli jsi skoro na konci stránky
  const isNearBottom = window.innerHeight + window.scrollY >= document.documentElement.scrollHeight - 40;

  // Pokud jsi skoro dole, aktivuj poslední sekci
  if (isNearBottom) {
    activeSection.value = sections[sections.length - 1].id;
    return;
  }

  sections.forEach(section => {
    const element = document.getElementById(section.id);
    if (element) {
      const { offsetTop, offsetHeight } = element;
      if (scrollPosition >= offsetTop && scrollPosition < offsetTop + offsetHeight) {
        activeSection.value = section.id;
      }
    }
  });
};

const scrollToSection = (id) => {
  const element = document.getElementById(id);
  // Přidej offset, aby to nescrollovalo těsně k hornímu okraji
  if (element) {
    const offsetPosition = element.offsetTop - 80; // 80px offset od vrchu
    window.scrollTo({
      top: offsetPosition,
      behavior: 'smooth'
    });
  }
};

onMounted(() => {
  window.addEventListener('scroll', handleScroll);
  handleScroll();
});

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll);
});
</script>