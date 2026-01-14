
<script setup>
import { BriefcaseIcon } from "lucide-vue-next";
</script>

<template>
  <section
    id="experience"
    class="min-h-screen bg-gradient-to-b from-indigo-50 via-white to-indigo-100 py-20 px-6 text-gray-800"
  >
    <div class="max-w-5xl mx-auto text-center mb-12">
      <h2
        class="text-4xl font-bold text-indigo-700 flex justify-center items-center gap-3"
      >
        <BriefcaseIcon class="w-8 h-8" /> Experiencia Profesional
      </h2>
      <p class="text-lg mt-3 text-gray-600">
        Más de una década de experiencia en entornos tecnológicos, combinando
        desarrollo frontend, buenas prácticas y colaboración en equipos ágiles.
      </p>
    </div>

    <div class="space-y-10 max-w-4xl mx-auto">
      <!-- Krell / Indra / BBVA -->
      <div
        class="bg-white shadow-lg hover:shadow-2xl transition-all duration-500 rounded-2xl p-8 border-l-4 border-blue-600 hover:translate-x-1"
      >
        <h3 class="text-2xl font-semibold text-indigo-700">
          Krell Consulting (para Indra) — Front-End Developer
        </h3>
        <p class="text-sm text-gray-500 mb-4">
          Diciembre 2025 – Actualidad · Proyecto BBVA · 100% remoto
        </p>
        <ul class="list-disc list-inside text-gray-700 leading-relaxed">
          <li>
            Desarrollo Front-End en el proyecto <strong>Cells</strong> para
            <strong>BBVA</strong>, basado en arquitectura de
            <strong>microfrontends</strong>.
          </li>
          <li>
            Implementación de componentes desacoplados, reutilizables y alineados
            con estándares corporativos.
          </li>
          <li>
            Desarrollo y mantenimiento de <strong>tests unitarios</strong> con
            <strong>Mocha</strong> y <strong>Chai</strong>.
          </li>
          <li>
            Trabajo en equipos multidisciplinares bajo metodologías ágiles,
            colaborando con perfiles de backend, QA y UX.
          </li>
        </ul>
      </div>

      <!-- Nalanda Global -->
      <div
        class="bg-white shadow-lg hover:shadow-2xl transition-all duration-500 rounded-2xl p-8 border-l-4 border-indigo-500 hover:translate-x-1"
      >
        <h3 class="text-2xl font-semibold text-indigo-700">
          Nalanda Global — Desarrollador Front-End
        </h3>
        <p class="text-sm text-gray-500 mb-4">2021 – 2025</p>
        <ul class="list-disc list-inside text-gray-700 leading-relaxed">
          <li>Desarrollo Front-End con Vue 2, Vue 3, jQuery y JSP.</li>
          <li>
            Participación clave en la incursión de Vue dentro de un proyecto
            legacy, creando componentes reutilizables para mejorar
            mantenibilidad y consistencia.
          </li>
          <li>
            Colaboración en la modernización completa de la web: nueva guía de
            estilos, revamp visual y optimización de la experiencia de usuario.
          </li>
          <li>
            Integración con APIs REST y AWS, control de versiones con GitLab y
            CI/CD con Jenkins.
          </li>
          <li>
            Trabajo coordinado con equipos de UX/UI y backend usando Figma y Jira.
          </li>
        </ul>
      </div>

      <!-- Carrefour E-Commerce -->
      <div
        class="bg-white shadow-lg hover:shadow-2xl transition-all duration-500 rounded-2xl p-8 border-l-4 border-emerald-500 hover:translate-x-1"
      >
        <h3 class="text-2xl font-semibold text-indigo-700">
          Carrefour — Desarrollador Web E-Commerce
        </h3>
        <p class="text-sm text-gray-500 mb-4">2018 – 2021</p>
        <ul class="list-disc list-inside text-gray-700 leading-relaxed">
          <li>
            Involucrado en los proyectos de la página de moda de Carrefour,
            Checkout y la versión moderna del e-commerce.
          </li>
          <li>
            Desarrollo Front-End con Vue.js en entorno de microservicios,
            integrando ElasticSearch y APIs REST.
          </li>
          <li>Colaboración con equipos DevOps bajo metodología Scrum.</li>
          <li>
            Optimización de rendimiento y mejora de experiencia de usuario en
            los flujos de compra.
          </li>
        </ul>
      </div>

      <!-- Servicios Financieros Carrefour -->
      <div
        class="bg-white shadow-lg hover:shadow-2xl transition-all duration-500 rounded-2xl p-8 border-l-4 border-orange-500 hover:translate-x-1"
      >
        <h3 class="text-2xl font-semibold text-indigo-700">
          Servicios Financieros Carrefour — Técnico Data Office / Informático
          Senior
        </h3>
        <p class="text-sm text-gray-500 mb-4">2007 – 2018</p>
        <ul class="list-disc list-inside text-gray-700 leading-relaxed">
          <li>Automatización de reportes con SQL Server, Python y Tableau.</li>
          <li>
            Desarrollo interno con Access y AuraPortal para mejorar procesos
            administrativos.
          </li>
          <li>
            Soporte técnico avanzado y coordinación con equipos de negocio.
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>

<style scoped>
section {
  animation: fadeInUp 1s ease-in-out;
}

@keyframes fadeInUp {
  0% {
    opacity: 0;
    transform: translateY(30px);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>
