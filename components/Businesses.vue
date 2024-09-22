<template>
  <div class="flex flex-col lg:px-[64px] lg:py-[128px] bg-[#EBF5FE]">
    <div class="flex flex-col lg:space-y-11">
      <p class="text-center text-2xl lg:text-5xl font-bold">
        Ways we've helped 15,000+ businesses save time, money, and resources
      </p>
      <div
        class="bg-white lg:rounded-[120px] grid grid-cols-1 lg:grid-cols-5 p-6 gap-4 lg:pb-[64px]"
      >
        <div
          class="rounded-[300px] border border-[#313CBD] bg-[#313CBD] py-2 px-5 cursor-pointer"
        >
          <p class="text-center text-sm font-medium uppercase">
            Employee relocation
          </p>
        </div>
        <div class="rounded-[300px] bg-[#EBF5FE] py-2 px-5 cursor-pointer">
          <p class="text-center text-sm font-medium uppercase">
            Global Payroll
          </p>
        </div>
        <div class="rounded-[300px] bg-[#EBF5FE] py-2 px-5 cursor-pointer">
          <p class="text-center text-sm font-medium uppercase">Compliance</p>
        </div>
        <div class="rounded-[300px] bg-[#EBF5FE] py-2 px-5 cursor-pointer">
          <p class="text-center text-sm font-medium uppercase">
            Merger & Acquisition
          </p>
        </div>
        <div class="rounded-[300px] bg-[#EBF5FE] py-2 px-5 cursor-pointer">
          <p class="text-center text-sm font-medium uppercase">Global hiring</p>
        </div>
      </div>
      <div class="flex flex-col lg:flex-row lg:space-x-[72px]">
        <div class="flex-1 space-y-4">
          <p
            class="lg:text-[32px] text-sm font-bold lg:leading-[45px] text-[#15357A]"
          >
            How Revolut streamlined employee relocation with Deel
          </p>
          <p class="lg:text-lg text-sm font-bold text-[#06122C]">
            “Through Deel, we’ve been able to hire more than 150 people so far,
            and we have also relocated more than 10 employees to countries like
            the UAE and Switzerland.”
          </p>
          <p class="lg:pb-[65px] text-[#06122C] font-bold text-lg">
            — Luka Besling, HR Manager at Revolut
          </p>
          <p class="inline-flex space-x-1 text-[#2C71F0] text-lg">
            Explore Case Study
            <ArrowRightIcon class="shrink-0 h-6 w-6" />
          </p>
        </div>
        <div class="flex-1">
          <img
            src="/video.png"
            alt="businesses"
            class="h-[358px] w-[618px] shrink-0"
          />
        </div>
      </div>
    </div>
    <div></div>
  </div>
</template>
<script setup>
import { ArrowRightIcon } from '@heroicons/vue/24/outline';
</script>
