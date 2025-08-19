<template>
  <nav
    class="fixed w-full z-50 backdrop-blur-md bg-gradient-to-r from-blue-900/95 to-blue-700/95 shadow-2xl border-b border-white/10"
  >
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between items-center py-5">
        <!-- Remplace la partie logo dans ton <nav> -->
        <div class="flex items-center space-x-3 group cursor-pointer">
          <!-- Logo image optimisée -->
          <div
            class="relative w-18 h-18 rounded-xl overflow-hidden shadow-md ring-2 ring-white/20 transition-transform duration-300 group-hover:scale-105"
          >
            <img
              src="../assets/images/logo.png"
              alt="Logo Dr Rahal"
              class="w-full h-full object-contain"
            />
            <!-- Halo animé -->
            <div
              class="absolute inset-0 rounded-xl bg-blue-400/20 opacity-0 group-hover:opacity-100 transition-opacity duration-500 animate-pulse"
            ></div>
          </div>

          <!-- Texte logo -->
          <div>
            <div
              class="text-white text-xl font-bold tracking-wide leading-tight group-hover:text-blue-200 transition-colors duration-300"
            >
              Dr. Mohamed RAHAL
            </div>
            <div
              class="text-blue-200 text-xs font-medium group-hover:text-white transition-colors duration-300"
            >
              Gastro-entérologue
            </div>
          </div>
        </div>

  

        <!-- Desktop Menu avec indicateurs actifs -->
        <div class="hidden md:flex items-center space-x-1">
          <a
            @click="scrollTo('accueil')"
            class="relative text-white hover:text-blue-200 transition-all duration-300 font-medium cursor-pointer px-4 py-2 rounded-lg hover:bg-white/10 group"
          >
            <span class="relative z-10">Accueil</span>
            <div
              class="absolute inset-x-0 bottom-0 h-0.5 bg-white transform scale-x-0 group-hover:scale-x-100 transition-transform duration-300 rounded-full"
            ></div>
          </a>
          <a
            @click="scrollTo('services')"
            class="relative text-white hover:text-blue-200 transition-all duration-300 font-medium cursor-pointer px-4 py-2 rounded-lg hover:bg-white/10 group"
          >
            <span class="relative z-10">Services</span>
            <div
              class="absolute inset-x-0 bottom-0 h-0.5 bg-white transform scale-x-0 group-hover:scale-x-100 transition-transform duration-300 rounded-full"
            ></div>
          </a>
          <a
            @click="scrollTo('cabinet')"
            class="relative text-white hover:text-blue-200 transition-all duration-300 font-medium cursor-pointer px-4 py-2 rounded-lg hover:bg-white/10 group"
          >
            <span class="relative z-10">Le Cabinet</span>
            <div
              class="absolute inset-x-0 bottom-0 h-0.5 bg-white transform scale-x-0 group-hover:scale-x-100 transition-transform duration-300 rounded-full"
            ></div>
          </a>
          <a
            @click="scrollTo('contact')"
            class="relative text-white hover:text-blue-200 transition-all duration-300 font-medium cursor-pointer px-4 py-2 rounded-lg hover:bg-white/10 group"
          >
            <span class="relative z-10">Contact</span>
            <div
              class="absolute inset-x-0 bottom-0 h-0.5 bg-white transform scale-x-0 group-hover:scale-x-100 transition-transform duration-300 rounded-full"
            ></div>
          </a>

          <!-- Séparateur élégant -->
          <div class="w-px h-6 bg-white/30 mx-2"></div>

          <!-- Bouton CTA amélioré -->
          <button
            @click="scrollTo('contact')"
            class="relative overflow-hidden bg-white text-blue-900 px-6 py-2.5 rounded-full font-semibold hover:bg-blue-50 transform hover:scale-105 hover:-translate-y-0.5 transition-all duration-300 shadow-lg hover:shadow-xl group"
          >
            <span class="relative z-10 flex items-center space-x-2">
              <svg
                class="w-4 h-4"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M8 7V3m8 4V3m-9 8h10M5 21h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z"
                />
              </svg>
              <span>Prendre RDV</span>
            </span>
            <div
              class="absolute inset-0 bg-gradient-to-r from-blue-600 to-blue-500 opacity-0 group-hover:opacity-100 transition-opacity duration-300"
            ></div>
          </button>
        </div>

        <!-- Mobile menu button amélioré -->
        <div class="md:hidden">
          <button
            @click="toggleMenu"
            class="relative w-10 h-10 bg-white/20 backdrop-blur-sm rounded-lg flex items-center justify-center text-white focus:outline-none hover:bg-white/30 transition-all duration-300"
          >
            <svg
              class="w-6 h-6 transition-transform duration-300"
              :class="{ 'rotate-90': isMenuOpen }"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
            >
              <path
                v-if="!isMenuOpen"
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16M4 18h16"
              />
              <path
                v-else
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M6 18L18 6M6 6l12 12"
              />
            </svg>
          </button>
        </div>
      </div>

      <!-- Mobile Menu modernisé -->
      <div
        v-show="isMenuOpen"
        class="md:hidden backdrop-blur-md bg-blue-800/95 border-t border-white/10"
        style="animation: slideDown 0.3s ease-out"
      >
        <div class="py-4 space-y-1">
          <a
            @click="scrollTo('accueil')"
            class="flex items-center text-white hover:text-blue-200 hover:bg-white/10 px-4 py-3 cursor-pointer transition-all duration-300 rounded-lg mx-2 group"
          >
            <svg
              class="w-5 h-5 mr-3 opacity-70 group-hover:opacity-100"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6"
              />
            </svg>
            <span class="font-medium">Accueil</span>
          </a>
          <a
            @click="scrollTo('services')"
            class="flex items-center text-white hover:text-blue-200 hover:bg-white/10 px-4 py-3 cursor-pointer transition-all duration-300 rounded-lg mx-2 group"
          >
            <svg
              class="w-5 h-5 mr-3 opacity-70 group-hover:opacity-100"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M19.428 15.428a2 2 0 00-1.022-.547l-2.387-.477a6 6 0 00-3.86.517l-.318.158a6 6 0 01-3.86.517L6.05 15.21a2 2 0 00-1.806.547M8 4h8l-1 1v5.172a2 2 0 00.586 1.414l5 5c1.26 1.26.367 3.414-1.415 3.414H4.828c-1.782 0-2.674-2.154-1.414-3.414l5-5A2 2 0 009 10.172V5L8 4z"
              />
            </svg>
            <span class="font-medium">Services</span>
          </a>
          <a
            @click="scrollTo('cabinet')"
            class="flex items-center text-white hover:text-blue-200 hover:bg-white/10 px-4 py-3 cursor-pointer transition-all duration-300 rounded-lg mx-2 group"
          >
            <svg
              class="w-5 h-5 mr-3 opacity-70 group-hover:opacity-100"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M19 21V5a2 2 0 00-2-2H7a2 2 0 00-2 2v16m14 0h2m-2 0h-5m-9 0H3m2 0h5M9 7h1m-1 4h1m4-4h1m-1 4h1m-5 10v-5a1 1 0 011-1h2a1 1 0 011 1v5m-4 0h4"
              />
            </svg>
            <span class="font-medium">Le Cabinet</span>
          </a>
          <a
            @click="scrollTo('contact')"
            class="flex items-center text-white hover:text-blue-200 hover:bg-white/10 px-4 py-3 cursor-pointer transition-all duration-300 rounded-lg mx-2 group"
          >
            <svg
              class="w-5 h-5 mr-3 opacity-70 group-hover:opacity-100"
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
            <span class="font-medium">Contact</span>
          </a>

          <!-- Bouton RDV mobile -->
          <div class="px-2 pt-2">
            <button
              @click="scrollTo('contact')"
              class="w-full bg-white text-blue-900 px-4 py-3 rounded-lg font-semibold hover:bg-blue-50 transition-all duration-300 flex items-center justify-center space-x-2"
            >
              <svg
                class="w-4 h-4"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M8 7V3m8 4V3m-9 8h10M5 21h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z"
                />
              </svg>
              <span>Prendre Rendez-vous</span>
            </button>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>

<script setup>
import { ref } from "vue";

const isMenuOpen = ref(false);

function toggleMenu() {
  isMenuOpen.value = !isMenuOpen.value;
}

/**
 * Scroll with offset to avoid hiding target under fixed navbar.
 * Adjust `extraOffset` si tu veux plus ou moins d'espace.
 */
function scrollTo(sectionId) {
  const el = document.getElementById(sectionId);
  if (!el) return;

  const nav = document.querySelector("nav");
  const navHeight = nav ? nav.getBoundingClientRect().height : 0;
  const extraOffset = 12; // px de marge sous la navbar
  const top =
    window.scrollY + el.getBoundingClientRect().top - navHeight - extraOffset;

  window.scrollTo({ top, behavior: "smooth" });
  isMenuOpen.value = false; // ferme le menu mobile si ouvert
}
</script>
<style>
@keyframes slideDown {
  from {
    opacity: 0;
    transform: translateY(-10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>
