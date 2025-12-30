<script setup>
</script>

<template>
<main class="w-full">
    <section class="bg-green-700 text-white">
    <img
    class="w-full h-[600px] object-cover"
    src="@/assets/banner4.jpg"
    alt="FarmBora banner"
    />
    <div class="absolute inset-0 bg-black bg-opacity-50 h-[500px] md:h-[600px]">
      <div
        class="absolute inset-0 flex flex-col justify-center items-center text-center text-white px-4"
      >
        <h1 class="text-4xl md:text-6xl font-bold mb-4">
          Contact Us
        </h1>

        <p class="text-lg text-green-100 max-w-3xl mx-auto">
          Have a question, need support, or want to partner with FarmBora?
          We’re here to help.
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
    <!-- CONTACT CONTENT -->
    <section class="py-16 bg-white">
      <div class="max-w-7xl mx-auto px-4 grid md:grid-cols-2 gap-12">

        <!-- CONTACT INFO -->
        <div>
          <h2 class="text-2xl font-bold mb-4">
            Get in Touch
          </h2>
          <p class="text-gray-700 mb-6">
            Whether you’re a farmer, buyer, or organization, our team is ready
            to support you and answer any questions you may have.
          </p>

          <ul class="space-y-4 text-gray-700">
            <li>
              <strong>Location:</strong><br />
              123 Tom Mboya Street,<br />
              Nairobi, Kenya
            </li>

            <li>
              <strong>Phone:</strong><br />
              +254 700 000 000
            </li>

            <li>
              <strong>Email:</strong><br />
              info@farmbora.com
            </li>
          </ul>

          <p class="mt-6 text-sm text-gray-500">
            We respond within 24 hours on business days.
          </p>
        </div>

        <div>
          <h2 class="text-2xl font-bold mb-4">
            Send Us a Message
          </h2>

          <form class="space-y-4"   action="https://formspree.io/f/mlgeknkk" method="POST">
            <div class="flex flex-col md:flex-row justify-between gap-5">
              <div class="flex-1">
              <label class="block text-sm font-medium text-gray-700 mb-1">
                First Name *
              </label>
              <input
                type="text"
                required
                name="first name"
                placeholder="e.g. John"
                class="w-full border rounded-lg px-4 py-2 focus:outline-none focus:ring-2 focus:ring-green-600"
              />
              </div>
              <div class="flex-1">
              <label class="block text-sm font-medium text-gray-700 mb-1">
                Last Name
              </label>
              <input
                type="text"
                name="last name"
                placeholder="e.g. Doe"
                class="w-full border rounded-lg px-4 py-2 focus:outline-none focus:ring-2 focus:ring-green-600"
              />
              </div>
            </div>

            <div>
              <label class="block text-sm font-medium text-gray-700 mb-1">
                Phone Number *
              </label>
              <input
                type="tel"
                required
                name="phone"
                placeholder="+254 7xx xxx xxx"
                class="w-full border rounded-lg px-4 py-2 focus:outline-none focus:ring-2 focus:ring-green-600"
              />  
            </div>

            <div>
              <label class="block text-sm font-medium text-gray-700 mb-1">
                Email Address
              </label>
              <input
                type="email"
                name="email"
                placeholder="you@example.com"
                class="w-full border rounded-lg px-4 py-2 focus:outline-none focus:ring-2 focus:ring-green-600"
              />
            </div>

            <div>
              <label class="block text-sm font-medium text-gray-700 mb-1">
                Message *
              </label>
              <textarea
                rows="5"
                required
                name="message"
                placeholder="How can we help you?"
                class="w-full border rounded-lg px-4 py-2 focus:outline-none focus:ring-2 focus:ring-green-600"
              ></textarea>
            </div>

            <button
              type="submit"
              class="bg-green-700 text-white px-6 py-3 rounded-lg font-semibold hover:bg-green-800 transition w-full"
            >
              Send Message
            </button>
          </form>
        </div>

      </div>
    </section>

    <section class="py-16 bg-green-700 text-center">
      <h2 class="text-2xl font-bold mb-4 text-gray-50">
        Support for Farmers Comes First
      </h2>
      <p class="text-gray-50 max-w-3xl mx-auto">
        FarmBora is committed to helping farmers make informed decisions,
        not blind guesses. If you need help accessing prices, buyers, or market
        insights, reach out anytime.
      </p>
    </section>

  </main>
</template>
