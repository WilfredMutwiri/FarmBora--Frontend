<script setup></script>

<template>
  <div class="w-full mx-auto">
    <img
      class="w-full h-[600px] object-cover"
      src="@/assets/image1.jpg"
      alt="FarmBora banner"
    />
    <div class="absolute inset-0 bg-black bg-opacity-50 h-[600px] mt-20">
      <div
        class="absolute inset-0 flex flex-col justify-center items-center text-center text-white px-4"
      >
        <h1 class="text-4xl md:text-6xl font-bold mb-4">
          Welcome to Farm<span class="text-[#e6b101]">Bora</span>
        </h1>
        <p class="text-lg md:text-2xl mb-8">
          Sell Smarter. Earn More from Your Farm.
        </p>
        <p class="text-lg md:text-xl mb-8">
          FarmBora connects farmers directly to buyers and uses AI to predict
          prices, recommend the best selling time, and increase profits.
        </p>
        <div>
          <button
            class="bg-green-600 hover:bg-green-700 w-60 text-white font-bold py-3 px-6 rounded-full transition duration-300 border border-green-300 shadow-lg shadow-green-500/50"
          >
            Get Started as a Farmer
          </button>
          <button
            class="ml-4 bg-green-600 hover:bg-green-700 w-60 text-white font-bold py-3 px-6 rounded-full transition duration-300 border border-green-300 shadow-lg shadow-green-500/50"
          >
            Get Started as a Buyer
          </button>
        </div>
      </div>
    </div>
    
    <!-- problem section -->
    <div>
      <section class="w-11/12 mx-auto bg-white py-16">
          <h2 class="text-3xl md:text-4xl font-extrabold text-gray-900 mb-4 text-center">Why FarmBora Exists</h2>
          
          <div class="flex flex-col lg:flex-row justify-center gap-12">
            <div class="flex flex-col space-y-8">
            <div class="">
              <p class="text-lg text-gray-700 font-medium">
                Farming is hard, selling shouldn’t be.
              </p>
            </div>
            <p class="text-gray-600 leading-relaxed">
              Farmers work tirelessly to grow quality produce, yet many are
              forced to sell without knowing real market prices or accessing
              reliable buyers. Buyers, on the other hand, struggle to find
              consistent, high-quality supply from nearby farmers.
            </p>
            <div class="flex flex-row gap-8">
            <div>
              <h3 class="text-xl font-semibold text-gray-900 mb-3">
                Challenges Faced by Farmers
              </h3>
              <ul class="space-y-2 text-gray-600">
                <li>• Middlemen dictate unfair prices</li>
                <li>• No visibility into real market prices</li>
                <li>• Selling at the wrong time leads to losses</li>
                <li>• Limited access to trustworthy buyers</li>
              </ul>
            </div>

            <div>
              <h3 class="text-xl font-semibold text-gray-900 mb-3">
                Challenges Faced by Buyers
              </h3>
              <ul class="space-y-2 text-gray-600">
                <li>• Unreliable produce supply</li>
                <li>• Inconsistent crop quality</li>
                <li>• Difficulty finding nearby farmers</li>
              </ul>
            </div>
            </div>

            <div class="bg-green-50 border-l-4 border-green-600 p-4 rounded-md">
              <p class="text-gray-700 font-medium">
                The problem isn’t production , it’s lack of market connection
                and intelligence. FarmBora bridges this gap using AI-powered
                insights and direct buyer–farmer connections.
              </p>
            </div>
            <div class="flex flex-col sm:flex-row gap-4 pt-4">
              <button
                class="bg-green-600 hover:bg-green-700 text-white font-semibold py-3 px-8 rounded-full transition shadow-lg shadow-green-600/30"
              >
                Join as a Farmer
              </button>
              <button
                class="border border-green-600 text-green-600 hover:bg-green-50 font-semibold py-3 px-8 rounded-full transition"
              >
                Join as a Buyer
              </button>
            </div>
          </div>
          <div class="h-full w-full lg:w-1/2">
          <img
            class="mt-12 w-full object-cover rounded-lg shadow-lg"
            src="@/assets/image2.jpg"
            alt="FarmBora community"
        </div>
          </div>
      </section>
    </div>
</div>
</template>