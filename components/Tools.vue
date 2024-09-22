<template>
  <div
    class="flex flex-col px-2 py-4 lg:py-[128px] lg:px-[64px] lg:space-y-[56px]"
  >
    <div>
      <p
        class="text-[#15357A] text-2xl lg:text-5xl font-bold lg:leading-[68px]"
      >
        See you later 16 different HR tools
      </p>
      <div class="flex flex-col lg:flex-row">
        <div class="flex-1">
          <p class="text--[#06122C] text-lg font-normal">
            We’re simplifying every aspect of managing a worldwide team, from
            benefits and equity to working visas and equipment. It’s one
            platform made to get you set up compliantly in just 5 minutes.
          </p>
        </div>
        <div class="flex-1">
          <div class="justify-end flex space-x-6">
            <img src="/back.svg" class="h-16 w-16" alt="back button" />
            <img src="/forward.svg" class="h-16 w-16" alt="forward button" />
          </div>
        </div>
      </div>
    </div>

    <div class="grid grid-cols-1 lg:grid-cols-4 pb-4 gap-6">
      <div class="bg-[#00AC6B] rounded-lg flex flex-col p-6">
        <div class="px-5 lg:pb-[18px]">
          <img src="/Group.png" class="h-[153px] w-[230px]" alt="tools" />
        </div>
        <p class="text-white text-2xl font-bold text-left pb-[36px]">
          Use Deel HR free to manage your global team in one system
        </p>
        <p
          class="text-base font-medium uppercase inline-flex space-x-[6px] text-white"
        >
          Learn More
          <ArrowRightIcon class="shrink-0 h-6 w-6" />
        </p>
      </div>
      <div class="bg-[#519AF4] rounded-lg flex flex-col p-6">
        <div class="px-5 lg:pb-[18px]">
          <img src="/hire.png" class="h-[153px] w-[230px]" alt="tools" />
        </div>
        <p class="text-white text-2xl font-bold text-left pb-[36px]">
          Hire or relocate team members with in-house visa support
        </p>
        <p
          class="text-base font-medium uppercase inline-flex space-x-[6px] text-white"
        >
          Learn More
          <ArrowRightIcon class="shrink-0 h-6 w-6" />
        </p>
      </div>
      <div class="bg-[#1C4396] rounded-lg flex flex-col p-6">
        <div class="px-5 lg:pb-[18px]">
          <img src="/Equipment.png" class="h-[153px] w-[230px]" alt="tools" />
        </div>
        <p class="text-white text-2xl font-bold text-left pb-[36px]">
          Send equipment worldwide, without the hassle
        </p>
        <p
          class="text-base font-medium uppercase inline-flex space-x-[6px] text-white"
        >
          Learn More
          <ArrowRightIcon class="shrink-0 h-6 w-6" />
        </p>
      </div>
      <div class="bg-[#F78400] rounded-lg flex flex-col p-6">
        <div class="px-5 lg:pb-[18px]">
          <img src="/Benefits.png" class="h-[153px] w-[230px]" alt="tools" />
        </div>
        <p class="text-white text-2xl font-bold text-left pb-[36px]">
          Offer country-specific benefits at competitive rates
        </p>
        <p
          class="text-base font-medium uppercase inline-flex space-x-[6px] text-white"
        >
          Learn More
          <ArrowRightIcon class="shrink-0 h-6 w-6" />
        </p>
      </div>
    </div>
    <div class="flex items-center mx-auto">
      <div class="border border-[#2F5EDD] rounded-[300px] px-4 py-6">
        <p class="text-[#2F5EDD] text-base font-medium uppercase">Get a demo</p>
      </div>
    </div>
  </div>
</template>
<script setup>
import { ArrowRightIcon } from '@heroicons/vue/24/solid';
</script>
