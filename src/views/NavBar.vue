<script setup>
    import { RouterLink} from 'vue-router'
    import{ref} from 'vue'
    const isOpen = ref(false);
</script>
<template>
<nav
    class="bg-gray-50 fixed w-full z-50 top-0 start-0 "
>
    <div
    class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4"
    >
    <a
        href="/"
        class="flex items-center space-x-3 rtl:space-x-reverse"
    >
        <img
        src="@/assets/logo.png"
        class="h-10"
        alt="Flowbite Logo"
        />
        <h1 class="text-3xl font-bold text-green-700">
            Farm<span class="text-[#e6b101]">Bora</span>
        </h1>
    </a>
    <div class="flex md:order-2 space-x-3 md:space-x-0 rtl:space-x-reverse">
        <button
        @click="isOpen = !isOpen"
        type="button"
        class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-body rounded-base md:hidden hover:bg-neutral-secondary-soft hover:text-heading focus:outline-none focus:ring-2 focus:ring-neutral-tertiary"
        aria-controls="navbar-sticky"
        aria-expanded="false"
        >
        <span class="sr-only">Open main menu</span>
        <svg
            class="w-6 h-6"
            aria-hidden="true"
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            fill="none"
            viewBox="0 0 24 24"
        >
            <path
            stroke="currentColor"
            stroke-linecap="round"
            stroke-width="2"
            d="M5 7h14M5 12h14M5 17h14"
            />
        </svg>
        </button>
    </div>
<div
:class="[
    'w-full md:flex md:w-auto md:order-1',
    isOpen ? 'block' : 'hidden'
]">
        <ul
        class="flex flex-col p-4 md:p-0 mt-4 font-medium  md:space-x-8 rtl:space-x-reverse md:flex-row md:mt-0  "
        >
        <li class="pt-2 hover:text-green-800 transition duration-300">
        <RouterLink :to="{ name: 'home' }">Home</RouterLink>
        </li>
        <li class="pt-2 hover:text-green-800 transition duration-300">
            <RouterLink :to="{ name: 'about' }">About</RouterLink>
        </li>
        <li class="pt-2 hover:text-green-800 transition duration-300">
            <RouterLink :to="{ name: 'market' }">Market</RouterLink>
        </li>
        <li class="pt-2 hover:text-green-800 transition duration-300">
            <RouterLink :to="{ name: 'services' }">Services</RouterLink>
        </li>
        <li class="pt-2 hover:text-green-800 transition duration-300">
        <RouterLink :to="{ name: 'contact' }">Contact</RouterLink>
        </li>
        <li>
        <button
        type="button"
        class="text-white bg-green-700 hover:bg-green-800 box-border border border-transparent focus:ring-4 focus:ring-green-300 shadow-xs font-medium leading-5 rounded-md text-sm px-3 py-2 focus:outline-none w-full text-center mt-5 md:mt-0 md:w-auto transition duration-300"
        >
        Get started
        </button>
        </li>
        </ul>
    </div>
    </div>
</nav>
</template>
