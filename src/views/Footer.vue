<script setup>
    import { RouterLink} from 'vue-router'
    const currentYear = new Date().getFullYear();
</script>

<template>
<footer class="bg-neutral-900 text-neutral-300">
    <div class="w-11/12 px-4 sm:px-0 lg:px-8 py-10">
            <div class="flex flex-col sm:flex-row items-center justify-between gap-6">
            <div class="text-lg font-semibold text-white">
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
    </div>

    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
        <nav class="flex flex-col justify-center gap-6 text-sm">
        <h3 class="text-lg font-semibold text-white">Quick Links</h3>
        <ul
        class="flex flex-col md:p-0 font-medium"
        >
        <li class=" hover:text-green-800 transition duration-300">
        <RouterLink :to="{ name: 'home' }">Home</RouterLink>
        </li>
        <li class="pt-2 hover:text-green-800 transition duration-300">
            <RouterLink :to="{ name: 'about' }">About</RouterLink>
        </li>
        <li class="pt-2 hover:text-green-800 transition duration-300">
            <RouterLink :to="{ name: 'services' }">Services</RouterLink>
        </li>
        <li class="pt-2 hover:text-green-800 transition duration-300">
        <RouterLink :to="{ name: 'contact' }">Contact</RouterLink>
        </li>
        </ul>
    </nav>

    <div class="flex flex-col gap-2">
        <h3 class="text-lg font-semibold text-white mb-2">Location</h3>
        <p class="text-neutral-400">123 Tom Mboya St.<br/><span class="pl-10">Nairobi, Kenya</span></p>
        <p class="text-neutral-400">Phone: +254 700 000 00</p>
        <p class="text-neutral-400">Email: info@farmbora.com</p>
    </div>
    </div>
</div>

    <div class="border-t border-neutral-700 my-6"></div>

    <p class="text-center text-xs text-neutral-400">
        © {{ currentYear }} FarmBora - Empowering African Farmers with Technology
    </p>
    </div>
</footer>
</template>
