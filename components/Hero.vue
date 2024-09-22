<template>
  <div class="relative isolate overflow-hidden bg-[#00AC6B]">
    <!-- Navbar -->
    <Disclosure as="nav" class="bg-transparent" v-slot="{ open }">
      <div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
        <div class="relative flex h-16 items-center justify-between">
          <div class="absolute inset-y-0 left-0 flex items-center sm:hidden">
            <!-- Mobile menu button-->
            <DisclosureButton
              class="relative inline-flex items-center justify-center rounded-md p-2 text-gray-400 hover:bg-gray-300 hover:text-white focus:outline-none focus:ring-2 focus:ring-inset focus:ring-white"
            >
              <span class="absolute -inset-0.5" />
              <span class="sr-only">Open main menu</span>
              <Bars3Icon
                v-if="!open"
                class="block h-6 w-6"
                aria-hidden="true"
              />
              <XMarkIcon v-else class="block h-6 w-6" aria-hidden="true" />
            </DisclosureButton>
          </div>
          <div
            class="flex flex-1 items-center justify-center sm:items-stretch sm:justify-start"
          >
            <div class="flex flex-shrink-0 items-center">
              <img class="h-8 w-auto" src="/deel.png" alt="Your Company" />
            </div>
            <div class="hidden sm:ml-6 sm:block">
              <div class="flex space-x-4">
                <a
                  v-for="item in navigation"
                  :key="item.name"
                  :href="item.href"
                  :class="[
                    item.current
                      ? 'bg-transparent text-white'
                      : 'text-white hover:text-lg',
                    'rounded-md px-3 py-2 text-sm font-medium',
                  ]"
                  :aria-current="item.current ? 'page' : undefined"
                  >{{ item.name }}</a
                >
              </div>
            </div>
          </div>
        </div>
      </div>

      <DisclosurePanel class="sm:hidden">
        <div class="space-y-1 px-2 pb-3 pt-2">
          <DisclosureButton
            v-for="item in navigation"
            :key="item.name"
            as="a"
            :href="item.href"
            :class="[
              item.current
                ? 'bg-gray-900 text-white'
                : 'text-gray-300 hover:bg-gray-700 hover:text-white',
              'block rounded-md px-3 py-2 text-base font-medium',
            ]"
            :aria-current="item.current ? 'page' : undefined"
            >{{ item.name }}</DisclosureButton
          >
        </div>
      </DisclosurePanel>
    </Disclosure>

    <div class="mx-auto max-w-7xl px-8 sm:flex">
      <div
        class="mx-auto max-w-2xl flex-shrink-0 lg:mx-0 lg:max-w-xl lg:pt-[120px]"
      >
        <h1 class="text-white text-2xl sm:text-[64px] font-bold leading-[67px]">
          Everything you need to scale a global team
        </h1>
        <p class="mt-4 text-[20px] leading-8 font-medium text-white">
          IcPay helps thousands of companies expand globally with unmatched
          speed and flexibility. It's global hiring, HR and payroll in just one
          system.
        </p>

        <button
          type="button"
          class="relative inline-flex items-center rounded-xl bg-[#2C71F0] mt-8 px-4 py-2 text-md font-normal text-white hover:bg-bg-[#2C71F0] focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-[#2C71F0]"
        >
          Get started
        </button>
      </div>
      <div class="mx-auto mt-16 flex max-w-[644px]">
        <div class="max-w-3xl flex-none sm:max-w-5xl lg:max-w-none">
          <img
            src="/desktop_interface_v1.png"
            alt="Desktop Interface"
            width="615"
            height="615"
            class="w-[615px] rounded-md"
          />
        </div>
      </div>
    </div>

    <!-- Logo cloud -->
    <div class="my-8 max-w-full px-6 sm:mt-16 lg:mx-[62px]">
      <h2 class="text-center text-lg font-bold leading-[28px] text-white">
        Used by 15,000+ businesses from small startups to household names
      </h2>
      <div
        class="mx-auto mt-10 grid max-w-lg grid-cols-4 items-center gap-x-8 gap-y-10 sm:max-w-xl sm:grid-cols-6 sm:gap-x-10 lg:mx-0 lg:max-w-none lg:grid-cols-5"
      >
        <img
          class="col-span-2 max-h-12 w-full object-contain lg:col-span-1"
          src="https://tailwindui.com/img/logos/158x48/transistor-logo-white.svg"
          alt="Transistor"
          width="158"
          height="48"
        />
        <img
          class="col-span-2 max-h-12 w-full object-contain lg:col-span-1"
          src="https://tailwindui.com/img/logos/158x48/reform-logo-white.svg"
          alt="Reform"
          width="158"
          height="48"
        />
        <img
          class="col-span-2 max-h-12 w-full object-contain lg:col-span-1"
          src="https://tailwindui.com/img/logos/158x48/tuple-logo-white.svg"
          alt="Tuple"
          width="158"
          height="48"
        />
        <img
          class="col-span-2 max-h-12 w-full object-contain sm:col-start-2 lg:col-span-1"
          src="https://tailwindui.com/img/logos/158x48/savvycal-logo-white.svg"
          alt="SavvyCal"
          width="158"
          height="48"
        />
        <img
          class="col-span-2 col-start-2 max-h-12 w-full object-contain sm:col-start-auto lg:col-span-1"
          src="https://tailwindui.com/img/logos/158x48/statamic-logo-white.svg"
          alt="Statamic"
          width="158"
          height="48"
        />
      </div>
    </div>
  </div>
</template>

<script setup>
import {
  Disclosure,
  DisclosureButton,
  DisclosurePanel,
  Menu,
  MenuButton,
  MenuItem,
  MenuItems,
} from '@headlessui/vue';
import { Bars3Icon, BellIcon, XMarkIcon } from '@heroicons/vue/24/outline';

const navigation = [
  { name: 'Platform', href: '#platform', current: true },
  { name: 'Use cases', href: '#usecase', current: false },
  { name: 'Why icpay', href: '#whyicpay', current: false },
  { name: 'Pricing', href: '#pricing', current: false },
  { name: 'Resources', href: '#resources', current: false },
];
</script>
