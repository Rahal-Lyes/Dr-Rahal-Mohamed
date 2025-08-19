<template>
  <!-- Navigation -->
  <Navigation />

  <!-- Hero Section -->
  <Accueil />

  <!-- Services Section -->
  <Services />

  <!-- Cabinet Section -->
  <Cabinet />
  <!-- Contact Section -->
  <Contact/>

  <!-- Footer -->
  <Footer/>
</template>
<script setup>
import { ref } from "vue";
import Navigation from "./components/Navigation.vue";
import Accueil from "./components/Accueil.vue";
import Services from "./components/Services.vue";
import Cabinet from "./components/Cabinet.vue";
import Contact from "./components/Contact.vue";
import Footer from "./components/Footer.vue";
const isMenuOpen = ref(false);
</script>
