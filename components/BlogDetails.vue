
<template>
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <!-- Title -->
      <h1 class="font-extrabold text-2xl sm:text-3xl md:text-4xl text-center py-6">
        {{ blog.description }}
      </h1>
  
      <!-- Blog Image -->
      <div class="w-full">
        <img class="h-120 w-full rounded-lg object-cover" :src="blog.image" :alt="blog.category">
      </div>
  
      <!-- Meta Information -->
      <div class="mt-8">
        <div class="flex flex-col sm:flex-row sm:items-center gap-4 sm:gap-10 text-center sm:text-left">
          <span class="text-slate-600 text-sm sm:text-lg uppercase">Posted by: {{ blog.name }}</span>
          <div class="flex items-center gap-2 text-sm sm:text-lg justify-center text-slate-600">
            <i class="material-icons">calendar_month</i>
            <span>{{ blog.date }}</span>
          </div>
          <span class="category p-1 text-sm sm:text-lg font-semibold">{{ blog.category }}</span>
        </div>
      </div>
  
      <!-- Blog Content -->
      <div class="mt-6">
        <p class="py-5 text-lg sm:text-xl leading-relaxed">{{ blog.body }}</p>
      </div>
    </div>
  </template>
  
  <script setup>
  const { blog } = defineProps(["blog"]);
  </script>
  