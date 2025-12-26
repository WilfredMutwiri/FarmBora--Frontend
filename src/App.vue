<script setup>
import { ref } from 'vue'
import { RouterLink, RouterView } from 'vue-router'

const isOpen = ref(false)
</script>

<template>
  <div>
    <header class="border-b border-gray-200 fixed top-0 w-full bg-white z-50">
      <div class="flex justify-between items-center p-5 w-full mx-auto lg:pr-20">
        <div class="flex justify-between items-center w-full">
        <div class="flex items-center">
            <img
              src="@/assets/logo.png"
              alt="FarmBora Logo"
              class="h-10 mr-2"
            />
            <h1 class="text-3xl font-bold text-green-700">
              Farm<span class="text-[#e6b101]">Bora</span>
            </h1>
          </div>
          <div>
          <button
            class="md:hidden focus:outline-none"
            @click="isOpen = !isOpen"
            aria-label="Toggle menu"
          >
            <svg
              class="w-7 h-7 text-green-700"
              fill="none"
              stroke="currentColor"
              stroke-width="2"
              viewBox="0 0 24 24"
            >
              <path stroke-linecap="round" stroke-linejoin="round"
                d="M4 6h16M4 12h16M4 18h16"
              />
            </svg>
          </button>
          </div>
        </div>
        <nav class="hidden md:flex gap-6 text-gray-900 text-lg font-semibold">
          <RouterLink :to="{ name: 'home' }">Home</RouterLink>
          <RouterLink :to="{ name: 'about' }">About</RouterLink>
          <RouterLink :to="{ name: 'services' }">Services</RouterLink>
          <RouterLink :to="{ name: 'pricing' }">Pricing</RouterLink>
          <RouterLink :to="{ name: 'contact' }">Contact</RouterLink>
        </nav>
      </div>
      <div
        v-show="isOpen"
        class="md:hidden bg-white border-t border-gray-200 shadow-lg"
      >
        <nav class="flex flex-col px-6 py-4 gap-4 text-lg font-semibold">
          <RouterLink @click="isOpen = false" :to="{ name: 'home' }">Home</RouterLink>
          <RouterLink @click="isOpen = false" :to="{ name: 'about' }">About</RouterLink>
          <RouterLink @click="isOpen = false" :to="{ name: 'services' }">Services</RouterLink>
          <RouterLink @click="isOpen = false" :to="{ name: 'pricing' }">Pricing</RouterLink>
          <RouterLink @click="isOpen = false" :to="{ name: 'contact' }">Contact</RouterLink>
        </nav>
      </div>
    </header>
    <main class="">
      <RouterView />
    </main>
  </div>
</template>

<style scoped>
nav a.router-link-exact-active {
  color: green;
}
</style>
