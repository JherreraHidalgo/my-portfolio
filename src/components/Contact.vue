<script setup>
import { Mail, Linkedin, Github, Phone } from "lucide-vue-next";
</script>

<template>
  <section
    id="contact"
    class="min-h-screen flex flex-col justify-center items-center bg-gradient-to-b from-slate-900 to-slate-800 text-white py-20 px-6"
  >
    <div class="text-center mb-12">
      <h2 class="text-4xl font-bold mb-4">Contacto</h2>
      <p class="text-slate-300 max-w-xl mx-auto">
        Si quieres ponerte en contacto conmigo para hablar de proyectos,
        colaboraciones o simplemente charlar sobre desarrollo, puedes hacerlo
        por cualquiera de estos medios:
      </p>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-2 gap-8 w-full max-w-3xl">
      <!-- Email -->
      <a
        href="mailto:javiherrera19@gmail.com"
        class="flex items-center gap-4 bg-slate-700/50 hover:bg-slate-700 transition-all duration-300 p-6 rounded-2xl shadow-lg hover:-translate-y-1"
      >
        <Mail class="w-8 h-8 text-blue-400" />
        <div>
          <p class="text-lg font-semibold">Correo</p>
          <p class="text-slate-300">javiherrera19@gmail.com</p>
        </div>
      </a>

      <!-- Teléfono -->
      <a
        href="tel:+34617693256"
        class="flex items-center gap-4 bg-slate-700/50 hover:bg-slate-700 transition-all duration-300 p-6 rounded-2xl shadow-lg hover:-translate-y-1"
      >
        <Phone class="w-8 h-8 text-green-400" />
        <div>
          <p class="text-lg font-semibold">Teléfono</p>
          <p class="text-slate-300">+34 617 69 32 56</p>
        </div>
      </a>

      <!-- LinkedIn -->
      <a
        href="https://www.linkedin.com/in/javier-herrera-hidalgo-8a76b5b4"
        target="_blank"
        class="flex items-center gap-4 bg-slate-700/50 hover:bg-slate-700 transition-all duration-300 p-6 rounded-2xl shadow-lg hover:-translate-y-1"
      >
        <Linkedin class="w-8 h-8 text-blue-500" />
        <div>
          <p class="text-lg font-semibold">LinkedIn</p>
          <p class="text-slate-300">/in/javier-herrera-hidalgo-8a76b5b4</p>
        </div>
      </a>

      <!-- GitHub -->
      <a
        href="https://github.com/JherreraHidalgo"
        target="_blank"
        class="flex items-center gap-4 bg-slate-700/50 hover:bg-slate-700 transition-all duration-300 p-6 rounded-2xl shadow-lg hover:-translate-y-1"
      >
        <Github class="w-8 h-8 text-gray-300" />
        <div>
          <p class="text-lg font-semibold">GitHub</p>
          <p class="text-slate-300">JherreraHidalgo</p>
        </div>
      </a>
    </div>
  </section>
</template>
