<script setup>
import { ref } from 'vue'
import { RouterView } from 'vue-router'
import NavBar from './views/NavBar.vue';
</script>

<template>
  <header>
  <NavBar />
  </header>
      <main class="">
      <RouterView />
    </main>
</template>
