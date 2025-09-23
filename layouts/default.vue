<template>
  <div class="min-h-screen bg-white">
    <nav class="fixed top-0 left-0 right-0 z-50 bg-white/90 backdrop-blur-sm border-b border-gray-100">
      <div class="max-w-6xl mx-auto px-6 py-4">
        <div class="flex justify-between items-center">
          <NuxtLink to="/" class="text-2xl font-bold text-gray-900">
            Khode
          </NuxtLink>
          <div class="hidden md:flex space-x-8">
            <NuxtLink to="/" class="text-gray-600 hover:text-gray-900 transition-colors">Home</NuxtLink>
            <NuxtLink to="/services" class="text-gray-600 hover:text-gray-900 transition-colors">Services</NuxtLink>
            <NuxtLink to="/about" class="text-gray-600 hover:text-gray-900 transition-colors">About</NuxtLink>
            <NuxtLink to="/contact" class="text-gray-600 hover:text-gray-900 transition-colors">Contact</NuxtLink>
          </div>
        </div>
      </div>
    </nav>
    
    <main class="pt-20">
      <slot />
    </main>
    
    <footer class="bg-gray-50 border-t border-gray-100">
      <div class="max-w-6xl mx-auto px-6 py-12">
        <div class="text-center text-gray-600">
          <p>&copy; 2025 Khode. All rights reserved.</p>
        </div>
      </div>
    </footer>
  </div>
</template>
