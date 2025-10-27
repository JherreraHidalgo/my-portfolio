<template>
  <section
    id="skills"
    class="py-20 bg-gradient-to-r from-indigo-50 via-purple-50 to-blue-50 text-gray-800"
  >
    <div class="container mx-auto px-6">
      <h3
        class="text-4xl font-bold text-center text-indigo-800 mb-12 animate-fadeIn"
      >
        Habilidades Técnicas
      </h3>

      <!-- Lenguajes y Frameworks -->
      <div
        class="bg-white rounded-2xl shadow-lg p-8 mb-8 border-l-4 border-indigo-500 hover:shadow-2xl transition-all animate-fadeIn delay-100"
      >
        <h4 class="text-2xl font-semibold text-indigo-700 mb-4">
          Lenguajes y Frameworks
        </h4>
        <div class="flex flex-wrap gap-3 text-gray-700">
          <span class="tag">Java</span>
          <span class="tag">JavaScript (ES6)</span>
          <span class="tag">TypeScript</span>
          <span class="tag">Node.js</span>
          <span class="tag">Go</span>
          <span class="tag">HTML5</span>
          <span class="tag">CSS3</span>
          <span class="tag">Vue 2 / 3</span>
          <span class="tag">Spring / SpringBoot</span>
          <span class="tag">jQuery</span>
          <span class="tag">JSP</span>
        </div>
      </div>

      <!-- Bases de datos -->
      <div
        class="bg-white rounded-2xl shadow-lg p-8 mb-8 border-l-4 border-purple-500 hover:shadow-2xl transition-all animate-fadeIn delay-200"
      >
        <h4 class="text-2xl font-semibold text-purple-700 mb-4">
          Bases de Datos
        </h4>
        <div class="flex flex-wrap gap-3 text-gray-700">
          <span class="tag">MySQL</span>
          <span class="tag">PostgreSQL</span>
          <span class="tag">SQL Server</span>
          <span class="tag">MongoDB</span>
        </div>
      </div>

      <!-- Herramientas y Entornos -->
      <div
        class="bg-white rounded-2xl shadow-lg p-8 mb-8 border-l-4 border-blue-500 hover:shadow-2xl transition-all animate-fadeIn delay-300"
      >
        <h4 class="text-2xl font-semibold text-blue-700 mb-4">
          Herramientas y Entornos
        </h4>
        <div class="flex flex-wrap gap-3 text-gray-700">
          <span class="tag">Docker</span>
          <span class="tag">Jenkins</span>
          <span class="tag">GitHub</span>
          <span class="tag">GitLab</span>
          <span class="tag">Heroku</span>
          <span class="tag">NPM</span>
          <span class="tag">Tableau</span>
          <span class="tag">Figma</span>
          <span class="tag">Jira</span>
          <span class="tag">AuraPortal</span>
          <span class="tag">ElasticSearch</span>
          <span class="tag">Apache Kafka</span>
          <span class="tag">WebFOCUS</span>
        </div>
      </div>

      <!-- Ofimática y Otros -->
      <div
        class="bg-white rounded-2xl shadow-lg p-8 border-l-4 border-green-500 hover:shadow-2xl transition-all animate-fadeIn delay-400"
      >
        <h4 class="text-2xl font-semibold text-green-700 mb-4">
          Ofimática y Otros
        </h4>
        <div class="flex flex-wrap gap-3 text-gray-700">
          <span class="tag">Microsoft Office (nivel experto)</span>
          <span class="tag">Visio</span>
          <span class="tag">FileZilla</span>
          <span class="tag">SPSS Statistics & Modeler</span>
          <span class="tag">Hue / Impala</span>
          <span class="tag">CRM</span>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style scoped>
.tag {
  background: linear-gradient(to right, #e0e7ff, #ede9fe);
  border-radius: 9999px;
  padding: 6px 14px;
  font-size: 0.9rem;
  font-weight: 500;
  transition: all 0.3s ease;
}
.tag:hover {
  background: linear-gradient(to right, #c7d2fe, #ddd6fe);
  transform: scale(1.05);
}
</style>
