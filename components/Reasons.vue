<template>
  <div class="flex flex-col lg:pt-[132px] lg:pb-[128px]">
    <div class="flex flex-col space-y-6 lg:mx-[333px] pb-4 lg:pb-[67px]">
      <p
        class="text-[#15357A] text-center text-2xl lg:text-5xl font-bold lg:leading-[68px]"
      >
        There’s a whole world out there. Why not hire anywhere?
      </p>
      <p class="text-[#06122C] text-center text-base lg:text-lg font-normal">
        Tap into the most extensive coverage on the market and hire anywhere in
        five minutes using our 100+ Deel entities and visa support. Yep, your
        talent pool just got infinite.
      </p>
    </div>
    <div
      class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6 p-6 pb-4 lg:pb-[67px]"
    >
      <div
        v-for="(country, index) in countries"
        :key="index"
        class="relative bg-cover bg-center rounded-xl shadow-lg h-96 transform transition-transform hover:scale-105"
        :class="getStaggeredClass(index)"
        :style="{ backgroundImage: `url(${country.image})` }"
      >
        <div
          class="absolute top-4 left-4 text-white font-bold text-xl drop-shadow-lg"
        >
          {{ country.name }}
        </div>
        <div class="absolute bottom-4 left-4 flex justify-start space-x-2">
          <button
            class="bg-transparent border border-white text-white py-2 px-4 rounded-[147px] transition-colors"
          >
            EOR
          </button>
          <button
            class="bg-transparent border border-white text-white py-2 px-4 rounded-[147px] transition-colors"
          >
            Contractor
          </button>
        </div>
        <div class="absolute bottom-[-23px] rounded-full right-[13px]">
          <img src="/flag.png" class="h-12 w-12" alt="flags" />
        </div>
      </div>
    </div>

    <div class="border border-[#2F5EDD] rounded-[300px] mx-auto p-4">
      <p class="text-[#2F5EDD] text-base font-medium uppercase">
        Explore Coverage Details
      </p>
    </div>
  </div>
</template>

<script setup>
const countries = [
  { name: 'Nigeria', image: '/nigeria.png' },
  { name: 'Poland', image: '/poland.png' },
  { name: 'Switzerland', image: '/switzerland.png' },
  { name: 'France', image: '/france.png' },
  // Add more countries here...
];

// Function to get staggered class for each item based on its index
const getStaggeredClass = (index) => {
  // Return different margins for different cards
  const classes = [
    'mt-0', // No margin for the first one
    'mt-8', // Margin top 8 for second
    'mt-0', // Margin top 4 for third
    'mt-8', // Margin top 12 for fourth
  ];
  return classes[index % classes.length]; // Repeat the pattern
};
</script>

<style scoped>
/* Add custom CSS here if necessary */
</style>
