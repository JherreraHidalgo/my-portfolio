<template>
  <div class="font-sans text-gray-800">
    <header
      class="bg-gradient-to-r from-blue-500 to-purple-600 text-white shadow-lg sticky top-0 z-50"
    >
      <div
        class="container mx-auto flex justify-between items-center py-4 px-6"
      >
        <h1 class="text-2xl font-bold tracking-wide">Javier Herrera Hidalgo</h1>
        <nav>
          <ul class="flex space-x-6 text-white">
            <li>
              <a href="#about" class="hover:text-yellow-300 transition"
                >Sobre mí</a
              >
            </li>
            <li>
              <a href="#experience" class="hover:text-yellow-300 transition"
                >Experiencia</a
              >
            </li>
            <li>
              <a href="#education" class="hover:text-yellow-300 transition"
                >Formación</a
              >
            </li>
            <li>
              <a href="#skills" class="hover:text-yellow-300 transition"
                >Habilidades</a
              >
            </li>
            <li>
              <a href="#contact" class="hover:text-yellow-300 transition"
                >Contacto</a
              >
            </li>
          </ul>
        </nav>
      </div>
    </header>

    <Hero />
    <About />
    <Experience />
    <Education />
    <Skills />
    <Contact />
  </div>
</template>

<script setup>
import Hero from "./components/Hero.vue";
import About from "./components/About.vue";
import Experience from "./components/Experience.vue";
import Education from "./components/Education.vue";
import Skills from "./components/Skills.vue";
import Contact from "./components/Contact.vue";
</script>
