<template>
  <div>
    <!-- Hero Section -->
    <section class="min-h-screen flex items-center justify-center bg-gradient-to-br from-gray-50 to-white">
      <div class="max-w-6xl mx-auto px-6 text-center">
        <div class="mb-6 inline-block px-4 py-2 bg-blue-50 text-blue-700 rounded-full text-sm font-medium">
          Now accepting projects for Q4 2025
        </div>
        
        <h1 class="text-5xl md:text-7xl font-bold text-gray-900 mb-6 leading-tight">
          Strengthen your company with
          <span class="bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">
            powerful solutions
          </span>
        </h1>
        
        <p class="text-xl md:text-2xl text-gray-600 mb-8 max-w-3xl mx-auto leading-relaxed">
          We create powerful solutions to your needs.
          From websites to full applications, we bring your vision to life.
        </p>
        
        <div class="flex flex-col sm:flex-row gap-4 justify-center">
          <NuxtLink 
            to="/contact" 
            class="bg-gray-900 text-white px-8 py-4 rounded-lg font-semibold hover:bg-gray-800 transition-colors"
          >
            Get a Quote Today
          </NuxtLink>
          <NuxtLink 
            to="/services" 
            class="border border-gray-300 text-gray-700 px-8 py-4 rounded-lg font-semibold hover:border-gray-400 transition-colors"
          >
            View Our Work
          </NuxtLink>
        </div>
      </div>
    </section>

    <!-- CTA Section -->
    <section class="py-24 bg-gray-900">
      <div class="max-w-4xl mx-auto px-6 text-center">
        <h2 class="text-4xl font-bold text-white mb-6">
          Ready to transform your digital presence?
        </h2>
        <p class="text-xl text-gray-300 mb-8">
          Let's discuss your project and see how we can help bring your vision to life.
        </p>
        <NuxtLink 
          to="/contact" 
          class="inline-block bg-white text-gray-900 px-8 py-4 rounded-lg font-semibold hover:bg-gray-100 transition-colors"
        >
          Start Your Project
        </NuxtLink>
      </div>
    </section>
  </div>
</template>

<script setup>
useSeoMeta({
  title: 'Khode - Digital Solutions',
  ogTitle: 'Khode - Digital Solutions',
  description: 'Strengthen your company with powerful solutions.',
  ogDescription: 'Strengthen your company with powerful solutions.',
})
</script>
