<script setup>
import HowItWorks from './HowItWorks.vue'; 
import ProblemView from './ProblemView.vue';
import AiAdvantage from './AiAdvantage.vue';
import TrustImpact from './TrustImpact.vue';
import WhoIsItFor from './WhoIsItFor.vue';
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
    <ProblemView/>
    <HowItWorks />
    <AiAdvantage />
    <TrustImpact />
    <WhoIsItFor />
    <div>
      <section class="w-full py-20 bg-gradient-to-r from-green-700 via-green-600 to-green-700">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center text-white">
      
      <h2 class="text-3xl md:text-4xl font-extrabold mb-4">
        Ready to farm smarter?
      </h2>

      <p class="text-lg md:text-xl text-green-100 max-w-2xl mx-auto mb-10">
        Join farmers and buyers using AI to trade smarter, reduce losses,
        and earn more from every harvest.
      </p>

      <div class="flex flex-col sm:flex-row justify-center gap-4">
        <button
          class="bg-white text-green-700 hover:bg-green-100 font-semibold py-3 px-8 rounded-full transition shadow-lg">
          Join as a Farmer
        </button>

        <button
          class="border border-white text-white hover:bg-white/10 font-semibold py-3 px-8 rounded-full transition">
          Join as a Buyer
        </button>
      </div>
    </div>
  </section>
    </div>
</div>
</template>