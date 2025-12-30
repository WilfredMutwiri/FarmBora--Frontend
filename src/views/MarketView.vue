<script setup>
import { ref, computed } from "vue";
const products = [
{
    id: 1,
    name: "Fresh Maize",
    price: "KES 3,500 per bag",
    description: "Dry, well-sorted maize harvested this season.",
    image: "/images/maize.jpg",
    farmer: "John Mwangi",
    phone: "+254 712 345 678",
    category: "Cereals",
},
{
    id: 2,
    name: "Irish Potatoes",
    price: "KES 60 per kg",
    description: "High-quality potatoes suitable for retail and processing.",
    image: "/images/potatoes.jpg",
    farmer: "Mary Wanjiku",
    phone: "+254 723 456 789",
    category: "Vegetables",
},
{
    id: 3,
    name: "Tomatoes",
    price: "KES 90 per kg",
    description: "Fresh, ripe tomatoes grown using sustainable practices.",
    image: "/images/tomatoes.jpg",
    farmer: "Peter Otieno",
    phone: "+254 734 567 890",
    category: "Vegetables",
},
{
    id: 4,
    name: "Green Beans",
    price: "KES 120 per kg",
    description: "Export-quality green beans available in bulk.",
    image: "/images/green-beans.jpg",
    farmer: "Amina Hassan",
    phone: "+254 745 678 901",
    category: "Cereals",
},
{
    id: 5,
    name: "Cabbages",
    price: "KES 50 per kg",
    description: "Fresh cabbages harvested this week.",
    image: "/images/cabbages.jpg",
    farmer: "Samuel Karanja",
    phone: "+254 756 789 012",
    category: "Vegetables",
},
{
    id: 6,
    name: "Carrots",
    price: "KES 80 per kg",
    description: "Crunchy and sweet carrots perfect for salads and cooking.",
    image: "/images/carrots.jpg",
    farmer: "Grace Njeri",
    phone: "+254 767 890 123",
    category: "Vegetables",
},
{
    id: 7,
    name: "Onions",
    price: "KES 70 per kg",
    description: "Fresh onions with a strong flavor, ideal for cooking.",
    image: "/images/onions.jpg",
    farmer: "David Mwenda",
    phone: "+254 778 901 234",
    category: "Vegetables",
},
{
    id: 8,
    name: "Bananas",
    price: "KES 40 per kg",
    description: "Sweet and ripe bananas, perfect for snacking.",
    image: "/images/bananas.jpg",
    farmer: "Lucy Achieng",
    phone: "+254 789 012 345",
    category: "Fruits",
},
{
    id: 9,
    name: "Mangoes",
    price: "KES 150 per kg",
    description: "Juicy and flavorful mangoes in season.",
    image: "/images/mangoes.jpg",
    farmer: "Joseph Otieno",
    phone: "+254 790 123 456",
    category: "Fruits",
},
];

const selectedCategory = ref("All");

const categories = ["All", "Cereals", "Vegetables", "Fruits"," Herbs", "Legumes"," Tubers"," Nuts", "Spices"];

const filteredProducts = computed(() => {
if (selectedCategory.value === "All") {
    return products;
}
return products.filter(
    (product) => product.category === selectedCategory.value
);
});
</script>


<template>
<main class="w-full">
    <section class="bg-green-700 text-white">
    <img
    class="w-full h-[600px] object-cover"
    src="/images/banner5.jpg"
    alt="FarmBora banner"
    />
    <div class="absolute inset-0 bg-black bg-opacity-50 h-[600px]">
    <div
        class="absolute inset-0 flex flex-col justify-center items-center text-center text-white px-4"
    >
        <h1 class="text-4xl md:text-6xl font-bold mb-4">
        Farm<span class="text-[#e6b101]">Bora</span> Market
        </h1>

        <p class="text-lg text-green-100 max-w-3xl mx-auto">
        Browse fresh farm produce directly from verified farmers.
        Transparent prices. Direct contact. No middlemen.
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
    <h2 class="text-2xl font-bold mb-6">
    Available Farm Products
    </h2>

    <div class="flex flex-wrap gap-3 mb-10">
    <button
        v-for="category in categories"
        :key="category"
        @click="selectedCategory = category"
        :class="[
        'px-5 py-2 rounded-full border text-sm font-medium transition',
        selectedCategory === category
            ? 'bg-green-700 text-white border-green-700'
            : 'border-gray-300 text-gray-700 hover:bg-green-50'
        ]"
    >
        {{ category }}
    </button>
    </div>

    <div class="grid sm:grid-cols-2 lg:grid-cols-4 gap-8">
    <div
        v-for="product in filteredProducts"
        :key="product.id"
        class="border rounded-lg overflow-hidden hover:shadow-lg transition"
    >
    <img
        :src="product.image"
        :alt="product.name"
        class="w-full h-48 object-cover"
    />

    <div class="p-6">
        <h3 class="text-lg font-semibold mb-1">
            {{ product.name }}
        </h3>

        <p class="text-green-700 font-bold mb-2">
            {{ product.price }}
        </p>

        <p class="text-sm text-gray-600 mb-4">
            {{ product.description }}
        </p>

        <div class="border-t pt-4 text-sm">
            <p><strong>Farmer:</strong> {{ product.farmer }}</p>
            <p>
            <strong>Phone:</strong>
            <a
                :href="`tel:${product.phone}`"
                class="text-green-700 hover:underline"
            >
                {{ product.phone }}
            </a>
            </p>
        </div>
        </div>
    </div>
    </div>

    <p
    v-if="filteredProducts.length === 0"
    class="text-gray-500 mt-10 text-center"
    >
    No products available in this category.
    </p>
</div>
</section>

<section class="py-20 bg-gray-50 text-center">
    <h2 class="text-2xl md:text-3xl font-bold mb-4">
        Want to Sell or Source Produce?
    </h2>
    <p class="text-gray-700 max-w-2xl mx-auto mb-8">
        Join FarmBora to access real-time market prices, verified buyers,
        and AI-powered insights that help you trade smarter.
    </p>

    <div class="flex flex-col sm:flex-row justify-center gap-4">
        <button
        class="bg-green-700 text-white px-8 py-3 rounded-full font-semibold hover:bg-green-800 transition"
        >
        Join as a Farmer
        </button>
        <button
        class="border border-green-700 text-green-700 px-8 py-3 rounded-full font-semibold hover:bg-green-50 transition"
        >
        Join as a Buyer
        </button>
    </div>
    </section>

</main>
</template>
