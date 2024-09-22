<template>
  <div class="lg:pt-[128px] lg:px-[64px]">
    <div class="flex flex-col">
      <div class="flex flex-col space-y-[21px]">
        <p class="text-center text-2xl lg:text-5xl font-bold text-[#15357A]">
          The reasons to choose Deel are clear
        </p>
        <p class="text-center text-base lg:text-lg font-normal text-[#06122C]">
          Our guaranteed top-tier service and industry-leading worldwide
          coverage provide peace of mind for any global team. With Deel’s
          next-level automation and in-house infrastructure, quality always
          comes first for our customers.
        </p>
      </div>
      <div class="border border-[#2F5EDD] rounded-[300px] mx-auto p-4">
        <p class="text-[#2F5EDD] text-base font-medium uppercase">
          contact sales to book a demo
        </p>
      </div>
      <div class="grid grid-cols-1 lg:grid-cols-3 gap-8 p-6 pb-4 lg:pb-20">
<StatView title="1.25min" sub="First response time with 24/7 in-app support" />
<StatView title="200+" sub="In-house tax, payroll and legal specialists" />
<StatView title="100+" sub="Deel-owned entities worldwide to hire and pay anywhere" />
        </div>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-8 p-6 pb-4 lg:pb-20">
            <StatView title="86hrs" sub="Saved by customers monthly automating HR admin" />
<StatView title="15+" sub="Flexible payment methods to pay your team" />
<StatView title="$210,000+" sub="Of entity set up costs saved per country" />
      </div>
    </div>
  </div>
</template>
<script setup>
import StatView from './ui/StatView.vue';
</script>
