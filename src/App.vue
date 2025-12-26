<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div>
    <header>
      <div class="flex flex-row justify-between items-center p-5">
        <div class="flex flex-row items-center mr-10">
          <img src="@/assets/logo.png" alt="FarmBora Logo" class="h-10 inline-block mr-3"/>
          <h1 class="text-3xl font-bold text-green-700">Farm<span class="text-[#e6b101]">Bora</span></h1>
        </div>
        <nav class="flex flex-row gap-5 text-gray-900 text-lg font-semibold">
          <RouterLink :to="{name:'home'}">Home</RouterLink>
          <RouterLink :to="{name:'about'}">About</RouterLink>
          <RouterLink :to="{name:'services'}">Services</RouterLink>
          <RouterLink :to="{name:'pricing'}">Pricing</RouterLink>
          <RouterLink :to="{name:'contact'}">Contact</RouterLink>
        </nav>
      </div>
    </header>   
    <main>
      <RouterView />
    </main>
  </div>
</template>

<style scoped>
nav a.router-link-exact-active {
  color:green;
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

</style>
