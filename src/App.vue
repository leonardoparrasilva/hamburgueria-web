<template>
  <Navbar :logo="logo_src" alt="App Name" />
  <RouterView />
  <Footer />
</template>

<script setup>
import { RouterView } from 'vue-router'
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'

const logo_src = "/img/logo.png";
const app_name = "Meu Aplicativo";

</script>
