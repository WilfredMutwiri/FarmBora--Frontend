<script setup>
</script>

<template>
<main class="w-full">
    <section class="bg-green-700 text-white">
    <img
    class="w-full h-[600px] object-cover"
    src="@/assets/banner3.jpg"
    alt="FarmBora banner"
    />
    <div class="absolute inset-0 bg-black bg-opacity-50 h-[500px] md:h-[600px]">
    <div
        class="absolute inset-0 flex flex-col justify-center items-center text-center text-white px-4"
    >
        <h1 class="text-4xl md:text-6xl font-bold mb-4">
        Our Services
        </h1>
        <p class="text-lg text-green-100 max-w-3xl mx-auto">
        FarmBora provides AI-powered tools and direct market access that help
        farmers sell smarter and buyers source produce more efficiently.
        </p>
        <div class="flex flex-col md:flex-row gap-4 md:gap-10 mt-4 items-center justify-center">
        <button
            class="bg-green-600 hover:bg-green-700 w-64 text-white font-bold py-3 rounded-full transition duration-300 border border-green-300 shadow-lg shadow-green-500/50"
        >
            Get Started as a Farmer
        </button>
        <button
            class="bg-green-600 hover:bg-green-700 w-64 text-white font-bold py-3 rounded-full transition duration-300 border border-green-300 shadow-lg shadow-green-500/50"
        >
            Get Started as a Buyer
        </button>
        </div>
    </div>
    </div>
    </section>

    <section class="py-16 bg-white">
    <div class="max-w-7xl mx-auto px-4">
        <h2 class="text-2xl font-bold mb-10 text-center">
        What FarmBora Offers
        </h2>

        <div class="grid sm:grid-cols-2 lg:grid-cols-3 gap-8">
        <div class="p-6 border rounded-lg hover:shadow-md transition">
            <h3 class="font-semibold text-lg mb-2">Direct Farmer, Buyer Marketplace</h3>
            <p class="text-gray-600 text-sm leading-relaxed">
            Buy and sell produce directly without unnecessary middlemen.
            Farmers reach reliable buyers, while buyers access fresh produce
            from nearby farms.
            </p>
        </div>

        <div class="p-6 border rounded-lg hover:shadow-md transition">
            <h3 class="font-semibold text-lg mb-2">AI Price Forecasting</h3>
            <p class="text-gray-600 text-sm leading-relaxed">
            Predict future price trends for over 30 crops and know when to sell
            for maximum profit.
            </p>
        </div>

        <div class="p-6 border rounded-lg hover:shadow-md transition">
            <h3 class="font-semibold text-lg mb-2">Smart Buyer–Seller Matching</h3>
            <p class="text-gray-600 text-sm leading-relaxed">
            Our AI matches farmers and buyers based on location, demand,
            transaction history, and reliability.
        </p>
        </div>

        <div class="p-6 border rounded-lg hover:shadow-md transition">
            <h3 class="font-semibold text-lg mb-2">Real-Time Market Prices</h3>
            <p class="text-gray-600 text-sm leading-relaxed">
            Access up-to-date market prices from multiple regions to avoid
            selling blindly.
            </p>
        </div>

        <div class="p-6 border rounded-lg hover:shadow-md transition">
            <h3 class="font-semibold text-lg mb-2">SMS & USSD Services</h3>
            <p class="text-gray-600 text-sm leading-relaxed">
            Receive price alerts, recommendations, and updates on any phone —
            even without internet access.
            </p>
        </div>

        <div class="p-6 border rounded-lg hover:shadow-md transition">
            <h3 class="font-semibold text-lg mb-2">Weekly Market Intelligence</h3>
            <p class="text-gray-600 text-sm leading-relaxed">
            AI-generated reports provide insights on demand trends, price
            movements, and regional market activity.
            </p>
        </div>

        </div>
    </div>
    </section>

    <section class="py-16 bg-gray-50">
    <div class="max-w-6xl mx-auto px-4 grid md:grid-cols-2 gap-12">
        <div>
        <h2 class="text-2xl font-bold mb-4">Services for Farmers</h2>
        <ul class="space-y-3 text-gray-700">
            <li>• Know the best time to sell using AI forecasts</li>
            <li>• Access reliable buyers without middlemen</li>
            <li>• Receive SMS price alerts and market updates</li>
            <li>• Reduce post-harvest losses</li>
            <li>• Get expert agricultural guidance</li>
        </ul>
        </div>

        <div>
        <h2 class="text-2xl font-bold mb-4">Services for Buyers</h2>
        <ul class="space-y-3 text-gray-700">
            <li>• Find nearby farmers quickly</li>
            <li>• Access consistent, quality produce</li>
            <li>• Reduce sourcing time and costs</li>
            <li>• Transparent pricing and supply insights</li>
            <li>• Secure and trusted transactions</li>
        </ul>
        </div>

    </div>
    </section>

    <section class="py-16 bg-white">
    <div class="max-w-5xl mx-auto px-4 text-center">
        <h2 class="text-2xl font-bold mb-4">
        Built for African Agriculture
        </h2>
        <p class="text-gray-700 leading-relaxed">
        FarmBora is designed for the realities of African farming ,
        unpredictable markets, limited access to information, and reliance on
        basic mobile phones. Our services are simple, accessible, and powered
        by proven AI technologies already supporting hundreds of thousands of
        farmers globally.
        </p>
    </div>
    </section>

    <section class="py-20 bg-green-700 text-white text-center">
    <h2 class="text-3xl font-extrabold mb-4">
        Start Trading Smarter Today
    </h2>
    <p class="text-green-100 max-w-2xl mx-auto mb-8">
        Whether you are a farmer or a buyer, FarmBora gives you the tools to make
        better market decisions.
    </p>

    <div class="flex flex-col sm:flex-row justify-center gap-4">
        <button class="bg-white text-green-700 px-8 py-3 rounded-full font-semibold">
        Get Started as a Farmer
        </button>
        <button class="border border-white px-8 py-3 rounded-full font-semibold">
        Get Started as a Buyer
        </button>
    </div>
    </section>

</main>
</template>
