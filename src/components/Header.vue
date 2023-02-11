<template>
      <Disclosure as="nav" class="absolute w-full h-32 top-0 left-0 z-10" v-slot="{ open }">
        <div class="mx-auto max-w-7xl px-8 md:px-20 pt-6 md:pt-8">
          <div class="flex h-16 items-center justify-between">
            <div class="flex items-center">
              <div class="flex-shrink-0">
                <img class="h-6 w-24" src="/logo-white@2x.png" alt="Your Company" />
              </div>


            </div>

            <div class="hidden lg:block">

              <div class="hidden md:block">
                <div class="ml-10 flex items-baseline space-x-3">
                  <a v-for="item in navigation" :key="item.name" :href="item.href" :class="[item.current ? 'underline ' : 'opacity-80 hover:opacity-100', 'decoration-1 underline-offset-4 py-2.5 px-4 rounded-md text-base font-medium text-left font-roboto text-white hover:text-white hover:underline']" :aria-current="item.current ? 'page' : undefined">{{ item.name }}</a>
                  
                  <a class="decoration-1 underline-offset-4 rounded-md text-base font-medium text-left text-white hover:text-white hover:underline opacity-80 hover:opacity-100">
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" class="w-5 h-5 pt-1">
                      <path fill-rule="evenodd" d="M9 3.5a5.5 5.5 0 100 11 5.5 5.5 0 000-11zM2 9a7 7 0 1112.452 4.391l3.328 3.329a.75.75 0 11-1.06 1.06l-3.329-3.328A7 7 0 012 9z" clip-rule="evenodd" />
                    </svg>
                    </a>
                </div>
              </div>
            </div>

            
            <div class="-mr-6 flex lg:hidden">
              <!-- Mobile menu button -->
              <DisclosureButton class="inline-flex items-center justify-center rounded-md  text-white">
                <span class="sr-only">Open main menu</span>
                <Bars3Icon v-if="!open" class="block h-10 w-10" aria-hidden="true" />
                <XMarkIcon v-else class="block h-10 w-10" aria-hidden="true" />
              </DisclosureButton>
            </div>
          </div>
        </div>
  
        <DisclosurePanel class="lg:hidden">
          <div class="space-y-1 px-2 pt-2 pb-3 sm:px-3">
            <DisclosureButton v-for="item in navigation" :key="item.name" as="a" :href="item.href" :class="[item.current ? 'bg-gray-900 text-white' : 'text-gray-300 hover:bg-gray-700 hover:text-white', 'block px-3 py-2 rounded-md text-base font-medium']" :aria-current="item.current ? 'page' : undefined">{{ item.name }}</DisclosureButton>
          </div>
          <div class="border-t border-gray-700 pt-4 pb-3">
            <div class="flex items-center px-5">
              <div class="flex-shrink-0">
                <img class="h-10 w-10 rounded-full" :src="user.imageUrl" alt="" />
              </div>
              <div class="ml-3">
                <div class="text-base font-medium leading-none text-white">{{ user.name }}</div>
                <div class="text-sm font-medium leading-none text-gray-400">{{ user.email }}</div>
              </div>
              <button type="button" class="ml-auto flex-shrink-0 rounded-full bg-gray-800 p-1 text-gray-400 hover:text-white focus:outline-none focus:ring-2 focus:ring-white focus:ring-offset-2 focus:ring-offset-gray-800">
                <span class="sr-only">View notifications</span>
                <BellIcon class="h-6 w-6" aria-hidden="true" />
              </button>
            </div>
            <div class="mt-3 space-y-1 px-2">
              <DisclosureButton v-for="item in userNavigation" :key="item.name" as="a" :href="item.href" class="block rounded-md px-3 py-2 text-base font-medium text-gray-400 hover:bg-gray-700 hover:text-white">{{ item.name }}</DisclosureButton>
            </div>
          </div>
        </DisclosurePanel>
      </Disclosure>


  </template>
  
  <script setup>
  import { Disclosure, DisclosureButton, DisclosurePanel, Menu, MenuButton, MenuItem, MenuItems } from '@headlessui/vue'
  import { Bars3Icon, BellIcon, XMarkIcon } from '@heroicons/vue/24/outline'
  
  const user = {
    name: 'Tom Cook',
    email: 'tom@example.com',
    imageUrl:
      'https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80',
  }
  const navigation = [
    { name: 'Home', href: '#', current: true },
    { name: 'Features', href: '#', current: false },
    { name: 'Screenshots', href: '#', current: false },
    { name: 'Support', href: '#', current: false },
    { name: 'Blog', href: '#', current: false },
    { name: 'Pricing', href: '#', current: false },
    { name: 'Contact', href: '#', current: false },
  ]
  const userNavigation = [
    { name: 'Your Profile', href: '#' },
    { name: 'Settings', href: '#' },
    { name: 'Sign out', href: '#' },
  ]
  </script>