<template>
  <section id="services" class="py-20 bg-white">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <h2 class="text-4xl font-bold text-gray-900 mb-4">Nos Spécialités</h2>
        <p class="text-xl text-gray-600 max-w-3xl mx-auto">
          Des soins spécialisés en gastro-entérologie et hépatologie pour votre
          bien-être digestif
        </p>
      </div>

      <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
        <div
          v-for="service in services"
          :key="service.title"
          class="bg-gradient-to-br from-blue-50 to-white p-8 rounded-2xl shadow-lg hover:shadow-xl transform hover:-translate-y-2 transition-all duration-300 border border-blue-100"
        >
          <div
            class="w-16 h-16 bg-blue-600 rounded-xl flex items-center justify-center mb-6"
          >
            <div v-html="service.icon" class="text-white"></div>
          </div>
          <h3 class="text-xl font-semibold text-gray-900 mb-4">
            {{ service.title }}
          </h3>
          <p class="text-gray-600 leading-relaxed">{{ service.description }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>


const services = [
  {
    title: "Consultation Gastro-entérologie",
    description:
      "Diagnostic et traitement des pathologies digestives : troubles de l'estomac, intestins, foie et pancréas.",
    icon: '<svg class="w-8 h-8" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z" /></svg>',
  },
  {
    title: "Hépatologie",
    description:
      "Prise en charge spécialisée des maladies du foie : hépatites, cirrhose, stéatose hépatique.",
    icon: '<svg class="w-8 h-8" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z" /></svg>',
  },
  
];

</script>