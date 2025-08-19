<template>
  <section id="contact" class="py-20 bg-white">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <h2 class="text-4xl font-bold text-gray-900 mb-4">
          Contactez le Dr. Mohamed RAHAL
        </h2>
        <p class="text-xl text-gray-600 max-w-3xl mx-auto">
          Gastro-entérologue & Hépatologue – Cabinet à Bouira
        </p>
      </div>

      <div class="grid md:grid-cols-2 gap-12">
        <!-- Infos -->
        <div class="space-y-8">
          <!-- Adresse -->
          <div class="flex items-start space-x-4">
            <div
              class="w-12 h-12 bg-blue-600 rounded-lg flex items-center justify-center flex-shrink-0"
            >
              <svg
                class="w-6 h-6 text-white"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"
                />
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"
                />
              </svg>
            </div>
            <div>
              <h3 class="text-lg font-semibold text-gray-900 mb-2">Adresse</h3>
              <p class="text-gray-600">
                CITÉ 280 LOGEMENTS, PROPRIÉTÉ N° 12<br />
                Bouira, Algérie
              </p>
              <p class="text-gray-600 text-sm mt-1">
                Cabinet de Gastro-entérologie & Hépatologie
              </p>
            </div>
          </div>

          <!-- Téléphone -->
          <div class="flex items-start space-x-4">
            <div
              class="w-12 h-12 bg-blue-600 rounded-lg flex items-center justify-center flex-shrink-0"
            >
              <svg
                class="w-6 h-6 text-white"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"
                />
              </svg>
            </div>
            <div>
              <h3 class="text-lg font-semibold text-gray-900 mb-2">
                Téléphones
              </h3>
              <p class="text-gray-600">📞 0774 66 27 72</p>
              <p class="text-gray-600">📞 0553 51 70 41</p>
              <p class="text-gray-600 text-sm mt-1">
                Horaires : 09h00 – 17h00
              </p>
            </div>
          </div>

          <!-- Email -->
          <div class="flex items-start space-x-4">
            <div
              class="w-12 h-12 bg-blue-600 rounded-lg flex items-center justify-center flex-shrink-0"
            >
              <svg
                class="w-6 h-6 text-white"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M3 8l7.89 4.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"
                />
              </svg>
            </div>
            <div>
              <h3 class="text-lg font-semibold text-gray-900 mb-2">Email</h3>
              <p class="text-gray-600">contact@cabinet-rahal.dz</p>
              <p class="text-gray-600 text-sm mt-1">Réponse sous 24h</p>
            </div>
          </div>
        </div>

        <!-- Formulaire -->
        <div
          class="bg-gradient-to-br from-blue-50 to-white p-8 rounded-2xl shadow-lg"
        >
          <h3 class="text-2xl font-semibold text-gray-900 mb-6">
            Prendre Rendez-vous
          </h3>
          <form class="space-y-6">
            <div>
              <label class="block text-sm font-medium text-gray-700 mb-2">
                Nom complet
              </label>
              <input
                type="text"
                class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:ring-2 focus:ring-blue-500 focus:border-transparent outline-none transition-all duration-200"
              />
            </div>
            <div>
              <label class="block text-sm font-medium text-gray-700 mb-2">
                Téléphone
              </label>
              <input
                type="tel"
                class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:ring-2 focus:ring-blue-500 focus:border-transparent outline-none transition-all duration-200"
              />
            </div>
            <div>
              <label class="block text-sm font-medium text-gray-700 mb-2">
                Motif de consultation
              </label>
              <textarea
                rows="4"
                class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:ring-2 focus:ring-blue-500 focus:border-transparent outline-none transition-all duration-200 resize-none"
              ></textarea>
            </div>
            <button
              type="submit"
              class="w-full bg-blue-600 text-white py-3 rounded-lg font-semibold hover:bg-blue-700 transform hover:scale-105 transition-all duration-300 shadow-lg"
            >
              Envoyer la demande
            </button>
          </form>
        </div>
      </div>

      <!-- Horaires -->
      <div class="text-center mt-12">
        <h3 class="text-xl font-semibold text-gray-900 mb-2">Horaires</h3>
        <p class="text-gray-600">
          Ouvert du <strong>Lundi</strong> au <strong>Jeudi</strong> &nbsp;|
          <strong>Samedi</strong> & <strong>Dimanche</strong> &nbsp;de 09h00 à
          17h00
        </p>
        <p class="text-red-500 mt-1">Fermé le Vendredi</p>
      </div>
    </div>
  </section>
</template>
