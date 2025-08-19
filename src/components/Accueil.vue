<template>
  <section
    id="accueil"
    class="relative pt-20 bg-gradient-to-br from-blue-50 via-white to-blue-100 min-h-screen flex items-center overflow-hidden"
  >
    <!-- Formes géométriques d'arrière-plan -->
    <div class="absolute inset-0 overflow-hidden">
      <div
        class="absolute -top-40 -right-40 w-80 h-80 bg-blue-200/30 rounded-full blur-3xl floating-animation"
      ></div>
      <div
        class="absolute -bottom-40 -left-40 w-96 h-96 bg-blue-300/20 rounded-full blur-3xl pulse-slow"
      ></div>
      <div
        class="absolute top-20 left-20 w-32 h-32 bg-blue-400/20 rounded-full blur-2xl floating-animation"
        style="animation-delay: 2s"
      ></div>
      <div
        class="absolute bottom-40 right-20 w-24 h-24 bg-purple-300/20 rounded-full blur-xl pulse-slow"
        style="animation-delay: 1s"
      ></div>
    </div>

    <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-20">
      <div
        class="flex flex-col lg:flex-row items-center justify-between gap-12"
      >
        <!-- Contenu textuel -->
        <div class="lg:w-1/2 space-y-8">
          <!-- Badge professionnel -->
          <div
            class="inline-flex items-center px-6 py-3 bg-gradient-to-r from-blue-100 to-blue-50 rounded-full text-blue-800 font-medium text-sm shadow-lg border border-blue-200/50"
          >
            <svg
              class="w-5 h-5 mr-2 text-yellow-500"
              fill="currentColor"
              viewBox="0 0 20 20"
            >
              <path
                d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"
              />
            </svg>
            Spécialiste Certifié & Expérimenté
          </div>

          <h1
            class="text-4xl lg:text-6xl font-bold text-gray-900 leading-tight"
          >
            <span class="block">Cabinet de</span>
            <span
              class="text-blue-600 block bg-gradient-to-r from-blue-600 to-blue-800 bg-clip-text text-transparent"
            >
              Gastro-entérologie
            </span>
            <span class="text-blue-800 block">&amp; Hépatologie</span>
          </h1>

          <p class="text-xl text-gray-600 leading-relaxed max-w-lg">
            Dr. Mohamed RAHAL vous accueille dans son cabinet spécialisé pour
            des soins digestifs de qualité avec une approche personnalisée et
            moderne.
          </p>

          <!-- Stats rapides -->
          <div class="grid grid-cols-3 gap-6 py-6">
            <div
              class="text-center p-4 bg-white/50 backdrop-blur-sm rounded-xl border border-white/20 shadow-lg"
            >
              <div class="text-3xl font-bold text-blue-600 mb-1">10+</div>
              <div class="text-sm text-gray-600 font-medium">
                Années d'expérience
              </div>
            </div>
            <div
              class="text-center p-4 bg-white/50 backdrop-blur-sm rounded-xl border border-white/20 shadow-lg"
            >
              <div class="text-3xl font-bold text-green-600 mb-1">1000+</div>
              <div class="text-sm text-gray-600 font-medium">
                Patients traités
              </div>
            </div>
            <div
              class="text-center p-4 bg-white/50 backdrop-blur-sm rounded-xl border border-white/20 shadow-lg"
            >
              <div class="text-3xl font-bold text-purple-600 mb-1">98%</div>
              <div class="text-sm text-gray-600 font-medium">Satisfaction</div>
            </div>
          </div>

          <div class="flex flex-col sm:flex-row gap-4">
            <button
              @click="scrollTo('contact')"
              class="group relative overflow-hidden bg-gradient-to-r from-blue-600 to-blue-700 text-white px-8 py-4 rounded-xl font-semibold hover:from-blue-700 hover:to-blue-800 transform hover:scale-105 transition-all duration-300 shadow-lg"
            >
              <span
                class="relative z-10 flex items-center justify-center space-x-2"
              >
                <svg
                  class="w-5 h-5"
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
              </span>
            </button>
            <button
              @click="scrollTo('services')"
              class="group border-2 border-blue-600 text-blue-600 px-8 py-4 rounded-xl font-semibold hover:bg-blue-600 hover:text-white transition-all duration-300 flex items-center justify-center space-x-2 bg-white/80"
            >
              <svg
                class="w-5 h-5"
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
              <span>Nos Services</span>
            </button>
          </div>
        </div>

        <!-- Slider d'images -->
        <div class="lg:w-1/2 relative">
          <div class="relative w-full max-w-lg mx-auto">
            <!-- Container du slider -->
            <div class="relative overflow-hidden rounded-3xl shadow-2xl">
              <!-- Slides -->
              <div
                class="flex transition-transform duration-700 ease-in-out"
                :style="{ transform: `translateX(-${currentSlide * 100}%)` }"
              >
                <!-- Slide 1: Cabinet moderne avec photo -->
                <div class="w-full flex-shrink-0 relative">
                  <div
                    class="h-96 bg-gradient-to-br from-blue-600 to-blue-800 flex items-center justify-center"
                  >
                    <div class="text-center text-white p-8">
                      <div class="relative w-64 h-48 mb-6 mx-auto">
                        <!-- Photo du cabinet - remplacez src par votre image -->
                        <img
                          src="https://images.unsplash.com/photo-1551190822-a9333d879b1f?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80"
                          alt="Cabinet médical moderne"
                          class="w-full h-full object-cover rounded-2xl shadow-lg border-4 border-white/30 transform hover:scale-105 transition-transform duration-500"
                        />
                      </div>
                      <h3 class="text-2xl font-bold mb-2">Cabinet Moderne</h3>
                      <p class="text-blue-100">
                        Équipements de dernière génération pour des diagnostics
                        précis
                      </p>
                    </div>
                  </div>
                </div>

                <!-- Slide 2: Docteur professionnel -->
                <div class="w-full flex-shrink-0 relative">
                  <div
                    class="h-96 bg-gradient-to-br from-green-600 to-teal-700 flex items-center justify-center"
                  >
                    <div class="text-center text-white p-8">
                      <div class="relative w-64 h-48 mb-6 mx-auto">
                        <!-- Photo du cabinet - remplacez src par votre image -->
                        <img
                          src="../assets/images/accuille3.jpg"
                          alt="Spécialiste en Gastro-entérologie & Hépatologie"
                          class="w-full h-full object-cover rounded-2xl shadow-lg border-4 border-white/30 transform hover:scale-105 transition-transform duration-500"
                        />
                      </div>
                      <h3 class="text-2xl font-bold mb-2">Dr. Mohamed RAHAL</h3>
                      <p class="text-green-100">
                        Spécialiste en Gastro-entérologie & Hépatologie
                      </p>
                    </div>
                  </div>
                </div>

                <!-- Slide 3: Services médicaux -->
                <div class="w-full flex-shrink-0 relative">
                  <div
                    class="h-96 bg-gradient-to-br from-purple-600 to-indigo-700 flex items-center justify-center"
                  >
                    <div class="text-center text-white p-8">
                      <div class="relative w-64 h-48 mb-6 mx-auto">
                        <!-- Photo du cabinet - remplacez src par votre image -->
                        <img
                          src="../assets/images/accuille4.jpg"
                          alt="Soins Personnalisés"
                          class="w-full h-full object-cover rounded-2xl shadow-lg border-4 border-white/30 transform hover:scale-105 transition-transform duration-500"
                        />
                      </div>
                      <h3 class="text-2xl font-bold mb-2">
                        Soins Personnalisés
                      </h3>
                      <p class="text-purple-100">
                        Approche individualisée pour chaque patient
                      </p>
                    </div>
                  </div>
                </div>

                <!-- Slide 4: Technologies -->
                <div class="w-full flex-shrink-0 relative">
                  <div
                    class="h-96 bg-gradient-to-br from-blue-600 to-indigo-700 flex items-center justify-center"
                  >
                    <div class="text-center text-white p-8">
                      <div class="relative w-64 h-48 mb-6 mx-auto">
                        <!-- Photo du cabinet - remplacez src par votre image -->
                        <img
                          src="../assets/images/accuille5.jpg"
                          alt="Cabinet médical moderne et accueillant"
                          class="w-full h-full object-cover rounded-2xl shadow-lg border-4 border-white/30 transform hover:scale-105 transition-transform duration-500"
                        />
                      </div>
                      <h3 class="text-2xl font-bold mb-2">
                        Cabinet du Dr. Mohamed RAHAL
                      </h3>
                      <p class="text-blue-100">
                        Un espace moderne et chaleureux dédié à la
                        gastro-entérologie et à l’hépatologie
                      </p>
                    </div>
                  </div>
                </div>
              </div>

              <!-- Navigation du slider -->
              <button
                @click="previousSlide"
                class="absolute left-4 top-1/2 transform -translate-y-1/2 bg-white/20 backdrop-blur-sm text-white p-3 rounded-full hover:bg-white/30 transition-all duration-300"
              >
                <svg
                  class="w-6 h-6"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M15 19l-7-7 7-7"
                  />
                </svg>
              </button>
              <button
                @click="nextSlide"
                class="absolute right-4 top-1/2 transform -translate-y-1/2 bg-white/20 backdrop-blur-sm text-white p-3 rounded-full hover:bg-white/30 transition-all duration-300"
              >
                <svg
                  class="w-6 h-6"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M9 5l7 7-7 7"
                  />
                </svg>
              </button>
            </div>

            <!-- Indicateurs de slides -->
            <div class="flex justify-center space-x-3 mt-6">
              <button
                v-for="(slide, index) in slides"
                :key="index"
                @click="goToSlide(index)"
                :class="[
                  'transition-all duration-300 rounded-full',
                  currentSlide === index
                    ? 'w-8 h-3 bg-blue-600'
                    : 'w-3 h-3 bg-gray-300 hover:bg-blue-400',
                ]"
              ></button>
            </div>

            <!-- Éléments décoratifs -->
            <div
              class="absolute -z-10 -top-6 -right-6 w-72 h-72 bg-blue-200/30 rounded-full blur-3xl"
            ></div>
            <div
              class="absolute -z-10 -bottom-6 -left-6 w-64 h-64 bg-blue-300/20 rounded-full blur-2xl"
            ></div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script setup>
import { ref, onMounted, onBeforeUnmount } from "vue";

const currentSlide = ref(0);
const slides = ref([
  { title: "Cabinet Moderne", color: "blue" },
  { title: "Dr. RAHAL", color: "green" },
  { title: "Soins Personnalisés", color: "purple" },
  { title: "Technologies Avancées", color: "orange" },
]);

const autoSlideInterval = ref(null);

function nextSlide() {
  currentSlide.value = (currentSlide.value + 1) % slides.value.length;
}

function previousSlide() {
  currentSlide.value =
    (currentSlide.value - 1 + slides.value.length) % slides.value.length;
}

function goToSlide(index) {
  currentSlide.value = index;
}

function startAutoSlide() {
  stopAutoSlide();
  autoSlideInterval.value = setInterval(() => {
    nextSlide();
  }, 6000); // toutes les 6 secondes
}

function stopAutoSlide() {
  if (autoSlideInterval.value) {
    clearInterval(autoSlideInterval.value);
    autoSlideInterval.value = null;
  }
}

onMounted(() => {
  startAutoSlide();
});

onBeforeUnmount(() => {
  stopAutoSlide();
});

function scrollTo(sectionId) {
  const el = document.getElementById(sectionId);
  if (!el) return;

  const nav = document.querySelector("nav");
  const navHeight = nav ? nav.getBoundingClientRect().height : 0;
  const extraOffset = 12;
  const top =
    window.scrollY + el.getBoundingClientRect().top - navHeight - extraOffset;

  window.scrollTo({ top, behavior: "smooth" });
}
</script>
<style>
.floating-animation {
  animation: float 6s ease-in-out infinite;
}
@keyframes float {
  0%,
  100% {
    transform: translateY(0px);
  }
  50% {
    transform: translateY(-10px);
  }
}
.pulse-slow {
  animation: pulse 4s infinite;
}
.glass-effect {
  backdrop-filter: blur(10px);
  background: rgba(255, 255, 255, 0.1);
  border: 1px solid rgba(255, 255, 255, 0.2);
}
</style>
