<template>
    <NuxtLink
      :to="to"
      class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:ring-blue-300 font-medium rounded-lg text-sm px-3 py-2 text-center inline-flex items-center"
    >
      <slot />
    </NuxtLink>
  </template>
  
  <script setup>
  defineProps({
    to: {
      type: String,
      required: false,
      default: "#",
    },
  });
  </script>
  