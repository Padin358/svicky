<template>
  <div class="w-full h-24 bg-gradient-to-b from-black/80 to-black/0"></div>

  <div class="flex flex-col lg:flex-row flex-wrap justify-evenly gap-12 p-8 text-[#dfdfdf]">
    <!-- Svíčka KLASIK -->
    <div class="border border-gray-800 rounded-2xl p-6 max-w-sm w-full bg-white/5">
      <p class="text-4xl font-black mb-3">Svíčka KLASIK</p>
      <p class="text-lg mb-4 opacity-80">
        Základní chytrá svíčka s AI bez nutnosti předplatného.
        Elegantní, jednoduchá, spolehlivá — přesně to, co potřebuješ pro pohodovou atmosféru.
      </p>
      <div class="flex items-center justify-between mt-6">
        <p class="text-2xl font-bold">1 290 Kč</p>
        <button class="bg-white/10 hover:bg-white/20 transition px-4 py-2 rounded-lg border border-gray-700 cursor-pointer">
          Koupit
        </button>
      </div>
    </div>

    <!-- Svíčka PREMIUM -->
    <div class="border border-yellow-700 rounded-2xl p-6 max-w-sm w-full bg-gradient-to-b from-yellow-900/20 to-transparent">
      <p class="text-4xl font-black mb-3 text-yellow-400">Svíčka PREMIUM</p>
      <p class="text-lg mb-4 opacity-90">
        Pokročilá AI svíčka se systémem předplatného.
        Umí reagovat na náladu, hlas i prostředí — tvůj osobní světelný asistent.
      </p>
      <div class="flex items-center justify-between mt-6">
        <p class="text-2xl font-bold text-yellow-300">3 990 Kč</p>
        <button class="bg-yellow-400/10 hover:bg-yellow-400/20 transition px-4 py-2 rounded-lg border border-yellow-600 cursor-pointer">
          Koupit
        </button>
      </div>
    </div>
  </div>
</template>

<script setup>
</script>
