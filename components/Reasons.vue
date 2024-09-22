<template>
    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6 p-6">
      <div
        v-for="(country, index) in countries"
        :key="index"
        class="relative bg-cover bg-center rounded-xl shadow-lg h-96 transform transition-transform hover:scale-105"
        :class="getStaggeredClass(index)"
        :style="{ backgroundImage: `url(${country.image})` }"
      >
        <div class="absolute top-4 left-4 text-white font-bold text-xl drop-shadow-lg">
          {{ country.name }}
        </div>
        <div class="absolute bottom-4 left-4 right-4 flex justify-between space-x-2">
          <button class="bg-blue-600 text-white py-2 px-4 rounded-lg hover:bg-blue-800 transition-colors">EOR</button>
          <button class="bg-blue-600 text-white py-2 px-4 rounded-lg hover:bg-blue-800 transition-colors">Contractor</button>
        </div>
      </div>
    </div>
  </template>
  
  <script setup>
  const countries = [
    { name: "Nigeria", image: "/nigeria.png" },
    { name: "Poland", image: "/poland.png" },
    { name: "Switzerland", image: "/switzerland.png" },
    { name: "France", image: "/france.png" },
    // Add more countries here...
  ];
  
  // Function to get staggered class for each item based on its index
  const getStaggeredClass = (index) => {
    // Return different margins for different cards
    const classes = [
      'mt-0',   // No margin for the first one
      'mt-8',   // Margin top 8 for second
      'mt-0',   // Margin top 4 for third
      'mt-8',  // Margin top 12 for fourth
    ];
    return classes[index % classes.length]; // Repeat the pattern
  };
  </script>
  
  <style scoped>
  /* Add custom CSS here if necessary */
  </style>
  