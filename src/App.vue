<template>
  <div class="font-sans text-gray-800">
    <header
      class="bg-gradient-to-r from-blue-500 to-purple-600 text-white shadow-lg sticky top-0 z-50"
    >
      <div
        class="container mx-auto flex justify-between items-center py-4 px-6"
      >
        <h1 class="text-2xl font-bold tracking-wide">Javier Herrera Hidalgo</h1>

        <!-- Botón hamburguesa para móviles -->
        <button
          class="sm:hidden focus:outline-none"
          @click="menuOpen = !menuOpen"
        >
          <svg
            class="w-6 h-6"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M4 6h16M4 12h16M4 18h16"
            ></path>
          </svg>
        </button>

        <!-- Navbar -->
        <nav
          :class="{
            'hidden sm:flex': !menuOpen,
            'flex flex-col sm:flex-row space-y-2 sm:space-y-0 sm:space-x-6 mt-4 sm:mt-0': true,
          }"
        >
          <ul class="flex flex-col sm:flex-row sm:space-x-6">
            <li v-for="section in sectionsList" :key="section.id">
              <button
                @click="
                  showSection(section.id);
                  menuOpen = false;
                "
                class="hover:text-yellow-300 transition relative pb-1"
              >
                {{ section.label }}
                <span
                  class="absolute left-0 -bottom-1 w-0 h-1 bg-yellow-300 transition-all duration-300 group-hover:w-full"
                ></span>
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

const menuOpen = ref(false);

const sections = {
  hero: Hero,
  about: About,
  experience: Experience,
  education: Education,
  skills: Skills,
  contact: Contact,
};

const currentSectionComponent = ref(Hero);

const sectionsList = [
  { id: "about", label: "Sobre mí" },
  { id: "experience", label: "Experiencia" },
  { id: "education", label: "Formación" },
  { id: "skills", label: "Habilidades" },
  { id: "contact", label: "Contacto" },
];

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
  transition: opacity 0.5s ease, transform 0.5s ease;
}
.fade-slide-enter-from,
.fade-slide-leave-to {
  opacity: 0;
  transform: translateY(30px);
}
.fade-slide-enter-to,
.fade-slide-leave-from {
  opacity: 1;
  transform: translateY(0);
}
</style>
