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
          <ul class="flex space-x-6">
            <li>
              <button
                @click="showSection('about')"
                class="hover:text-yellow-300 transition"
              >
                Sobre mí
              </button>
            </li>
            <li>
              <button
                @click="showSection('experience')"
                class="hover:text-yellow-300 transition"
              >
                Experiencia
              </button>
            </li>
            <li>
              <button
                @click="showSection('education')"
                class="hover:text-yellow-300 transition"
              >
                Formación
              </button>
            </li>
            <li>
              <button
                @click="showSection('skills')"
                class="hover:text-yellow-300 transition"
              >
                Habilidades
              </button>
            </li>
            <li>
              <button
                @click="showSection('contact')"
                class="hover:text-yellow-300 transition"
              >
                Contacto
              </button>
            </li>
          </ul>
        </nav>
      </div>
    </header>

    <!-- Secciones con animación -->
    <transition name="fade-slide" mode="out-in">
      <component :is="currentSectionComponent" v-if="currentSectionComponent" />
    </transition>
  </div>
</template>

<script setup>
import { ref } from "vue";
import Hero from "./components/Hero.vue";
import About from "./components/About.vue";
import Experience from "./components/Experience.vue";
import Education from "./components/Education.vue";
import Skills from "./components/Skills.vue";
import Contact from "./components/Contact.vue";

const currentSection = ref(null);

const sections = {
  hero: Hero,
  about: About,
  experience: Experience,
  education: Education,
  skills: Skills,
  contact: Contact,
};

const currentSectionComponent = ref(Hero); // al cargar, se ve Hero

function showSection(section) {
  if (sections[section]) {
    currentSectionComponent.value = sections[section];
  }
}
</script>

<style>
/* Animación fade + slide */
.fade-slide-enter-active,
.fade-slide-leave-active {
  transition: all 0.5s ease;
}
.fade-slide-enter-from {
  opacity: 0;
  transform: translateY(20px);
}
.fade-slide-enter-to {
  opacity: 1;
  transform: translateY(0);
}
.fade-slide-leave-from {
  opacity: 1;
  transform: translateY(0);
}
.fade-slide-leave-to {
  opacity: 0;
  transform: translateY(20px);
}
</style>
