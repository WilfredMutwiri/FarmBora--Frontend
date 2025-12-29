<script setup>
import HowItWorks from './HowItWorks.vue'; 
import ProblemView from './ProblemView.vue';
</script>

<template>
  <div class="w-full mx-auto mt-20">
    <img
      class="w-full h-[600px] object-cover"
      src="@/assets/image1.jpg"
      alt="FarmBora banner"
    />
    <div class="absolute inset-0 bg-black bg-opacity-50 h-[500px] md:h-[600px] mt-20">
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
    
    <!-- problem section -->
    <ProblemView/>
    <!-- how it works -->
    <HowItWorks />
</div>
</template>