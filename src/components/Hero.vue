<template>
  <section
    class="bg-gradient-to-r from-purple-600 to-blue-500 text-white py-24 sm:py-32 text-center"
  >
    <h2 class="text-4xl sm:text-5xl font-bold mb-4">Desarrollador Front-End</h2>
    <p
      class="text-lg sm:text-xl mb-6 max-w-xs sm:max-w-2xl mx-auto leading-relaxed"
    >
      Especializado en
      <span class="font-semibold text-yellow-300">Vue.js</span>,
      <span class="font-semibold text-yellow-300">JavaScript</span>,
      <span class="font-semibold text-yellow-300">TypeScript</span> y
      tecnologías web modernas. Apasionado por interfaces accesibles y
      experiencias digitales eficientes.
    </p>
    <button
      @click="$refs.contactSection.scrollIntoView({ behavior: 'smooth' })"
      class="inline-block bg-yellow-400 text-purple-800 font-bold px-6 sm:px-8 py-2 sm:py-3 rounded-lg shadow-lg hover:bg-yellow-300 hover:scale-105 transition-transform duration-300"
    >
      Conecta conmigo
    </button>
  </section>
</template>

<script setup></script>
