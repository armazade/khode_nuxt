<template>
  <div class="min-h-screen">
    <nav class="fixed top-0 left-0 right-0 z-50">
      <div class="px-6 py-4">
        <div class="flex justify-between items-center">
          <NuxtLink to="/" class="text-2xl font-bold text-white">
            Khode
          </NuxtLink>
        </div>
      </div>
    </nav>

    <main>
      <slot />
    </main>

    <footer>
      <div class="px-6 py-4 text-center bg-black">
        <p class="text-gray-400">&copy; 2025 Khode. All rights reserved.</p>
      </div>
    </footer>
  </div>
</template>
<script setup lang="ts">
</script>