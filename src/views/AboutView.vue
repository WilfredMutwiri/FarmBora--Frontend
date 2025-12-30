<script setup>
</script>

<template>
  <main class="w-full">
    <section class="bg-green-700 text-white">
      <img
      class="w-full h-[600px] object-cover"
      src="@/assets/image3.jpg"
      alt="FarmBora banner"
    />
    <div class="absolute inset-0 bg-black bg-opacity-50 h-[600px]">
      <div
        class="absolute inset-0 flex flex-col justify-center items-center text-center text-white px-4"
      >
        <h1 class="text-4xl md:text-6xl font-bold mb-4">
          About Farm<span class="text-[#e6b101]">Bora</span>
        </h1>

        <p class="text-lg text-green-100 max-w-3xl mx-auto">
          Empowering African farmers with technology that connects, informs,
          and unlocks better income opportunities.
        </p>
        <div class="flex flex-col md:flex-row gap-4 md:gap-10 mt-5 items-center justify-center">
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
      <div class="w-11/12 mx-auto px-4">
        <h2 class="text-2xl font-bold text-gray-900 mb-4">
          Who We Are
        </h2>
        <p class="text-gray-700 leading-relaxed max-w-4xl">
          FarmBora is an agri-tech platform built to solve one of agriculture’s
          biggest challenges, access to reliable markets and accurate pricing
          information. While farmers work tirelessly to grow quality produce,
          many still sell at a loss due to lack of market visibility and
          dependence on middlemen.
          <br /><br />
          We exist to change that.
        </p>
      </div>
    </section>

    <section class="py-16 bg-gray-50">
      <div class="w-11/12 mx-auto px-4 grid md:grid-cols-2 gap-10">
        <div>
          <h3 class="text-xl font-semibold mb-3">The Challenge</h3>
          <p class="text-gray-700 leading-relaxed">
            Agriculture in Africa is not limited by production , it is limited
            by information, access, and connection. Farmers often sell without
            knowing the real market price, while buyers struggle to find
            consistent, nearby supply.
          </p>
        </div>
        <div>
          <h3 class="text-xl font-semibold mb-3">Our Solution</h3>
          <p class="text-gray-700 leading-relaxed">
            FarmBora bridges this gap by connecting farmers directly to buyers
            and providing AI-powered market insights that guide smarter selling,
            better timing, and fairer pricing.
          </p>
        </div>
      </div>
    </section>

    <!-- WHAT WE DO -->
    <section class="py-16 bg-white">
      <div class="w-11/12 mx-auto px-4">
        <h2 class="text-2xl font-bold mb-8">What We Do</h2>

        <div class="grid sm:grid-cols-2 md:grid-cols-3 gap-8">
          <div class="p-6 border rounded-lg">
            <h4 class="font-semibold mb-2">Direct Market Access</h4>
            <p class="text-sm text-gray-600">
              We remove unnecessary middlemen by connecting farmers and buyers
              directly.
            </p>
          </div>

          <div class="p-6 border rounded-lg">
            <h4 class="font-semibold mb-2">AI Price Forecasting</h4>
            <p class="text-sm text-gray-600">
              Our AI predicts price trends for over 30 crops, helping farmers
              choose the best time to sell.
            </p>
          </div>

          <div class="p-6 border rounded-lg">
            <h4 class="font-semibold mb-2">Smart Matching</h4>
            <p class="text-sm text-gray-600">
              Buyers and farmers are matched based on location, demand, and
              reliability.
            </p>
          </div>

          <div class="p-6 border rounded-lg">
            <h4 class="font-semibold mb-2">Market Intelligence</h4>
            <p class="text-sm text-gray-600">
              Weekly AI-generated reports provide insights on demand and price
              movements.
            </p>
          </div>

          <div class="p-6 border rounded-lg">
            <h4 class="font-semibold mb-2">SMS & USSD Access</h4>
            <p class="text-sm text-gray-600">
              Farmers can access price alerts and insights even without
              internet-enabled smartphones.
            </p>
          </div>

          <div class="p-6 border rounded-lg">
            <h4 class="font-semibold mb-2">Expert Support</h4>
            <p class="text-sm text-gray-600">
              Agricultural experts are available to guide farmers with
              data-backed advice.
            </p>
          </div>
        </div>
      </div>
    </section>

    <section class="py-16 bg-gray-50">
      <div class="w-11/12 mx-auto px-4">
        <h2 class="text-2xl font-bold mb-6">Our Impact</h2>
        <p class="text-gray-700 mb-8">
          FarmBora is built around real agricultural data and proven AI models
          already supporting over <strong>400,000 farmers globally</strong>.
          Our goal is to ensure African farmers earn more, waste less, and make
          confident decisions.
        </p>

        <div class="grid sm:grid-cols-3 gap-6 text-center">
          <div class="p-6 bg-white rounded-lg shadow">
            <p class="text-3xl font-bold text-green-700">75%</p>
            <p class="text-sm text-gray-600">
              of Kenyans depend on agriculture
            </p>
          </div>
          <div class="p-6 bg-white rounded-lg shadow">
            <p class="text-3xl font-bold text-green-700">67%</p>
            <p class="text-sm text-gray-600">
              higher earnings via direct access
            </p>
          </div>
          <div class="p-6 bg-white rounded-lg shadow">
            <p class="text-3xl font-bold text-green-700">AI</p>
            <p class="text-sm text-gray-600">
              reduces farming risks and guesswork
            </p>
          </div>
        </div>
      </div>
    </section>

    <section class="py-20 bg-green-700 text-white text-center">
      <h2 class="text-3xl font-extrabold mb-4">
        Join the Future of Farming
      </h2>
      <p class="text-green-100 max-w-2xl mx-auto mb-8">
        Whether you grow food or buy it, FarmBora helps you trade smarter,
        earn more, and plan with confidence.
      </p>

      <div class="flex flex-col sm:flex-row justify-center gap-4">
        <button class="bg-white text-green-700 px-8 py-3 rounded-full font-semibold">
          Join as a Farmer
        </button>
        <button class="border border-white px-8 py-3 rounded-full font-semibold">
          Join as a Buyer
        </button>
      </div>
    </section>

  </main>
</template>
