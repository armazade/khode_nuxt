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

    <!-- Services Preview -->
    <section class="py-24 bg-white">
      <div class="max-w-6xl mx-auto px-6">
        <div class="text-center mb-16">
          <h2 class="text-4xl font-bold text-gray-900 mb-4">What We Do</h2>
          <p class="text-xl text-gray-600 max-w-2xl mx-auto">
            We specialize in creating digital solutions that make your business stand out
          </p>
        </div>
        
        <div class="grid md:grid-cols-3 gap-8">
          <div class="text-center p-8 border border-gray-100 rounded-2xl hover:shadow-lg transition-shadow">
            <div class="w-16 h-16 bg-blue-100 rounded-2xl flex items-center justify-center mx-auto mb-6">
              <svg class="w-8 h-8 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.75 17L9 20l-1 1h8l-1-1-.75-3M3 13h18M5 17h14a2 2 0 002-2V5a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path>
              </svg>
            </div>
            <h3 class="text-xl font-semibold text-gray-900 mb-3">Web Development</h3>
            <p class="text-gray-600">Modern, responsive applications built with the latest technologies</p>
          </div>
          
          <div class="text-center p-8 border border-gray-100 rounded-2xl hover:shadow-lg transition-shadow">
            <div class="w-16 h-16 bg-purple-100 rounded-2xl flex items-center justify-center mx-auto mb-6">
              <svg class="w-8 h-8 text-purple-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 18h.01M8 21h8a2 2 0 002-2V5a2 2 0 00-2-2H8a2 2 0 00-2 2v14a2 2 0 002 2z"></path>
              </svg>
            </div>
            <h3 class="text-xl font-semibold text-gray-900 mb-3">Mobile Apps</h3>
            <p class="text-gray-600">Native and cross-platform mobile applications</p>
          </div>
          
          <div class="text-center p-8 border border-gray-100 rounded-2xl hover:shadow-lg transition-shadow">
            <div class="w-16 h-16 bg-green-100 rounded-2xl flex items-center justify-center mx-auto mb-6">
              <svg class="w-8 h-8 text-green-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path>
              </svg>
            </div>
            <h3 class="text-xl font-semibold text-gray-900 mb-3">Brand Identity</h3>
            <p class="text-gray-600">Complete branding solutions from logo to digital presence</p>
          </div>
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
  title: 'YourCompany - Digital Solutions',
  ogTitle: 'YourCompany - Digital Solutions',
  description: 'Strengthen your brand with memorable digital experiences tuned to your unique identity.',
  ogDescription: 'Strengthen your brand with memorable digital experiences tuned to your unique identity.',
})
</script>
