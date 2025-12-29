<script setup>
import { ref } from 'vue'
import { RouterView } from 'vue-router'
import NavBar from './views/NavBar.vue';
import Footer from './views/Footer.vue';
</script>

<template>
  <header>
  <NavBar />
  </header>
      <main class="">
      <RouterView />
    </main>
  <footer>
    <Footer />
  </footer>
</template>
