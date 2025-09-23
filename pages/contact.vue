<template>
  <div class="py-24">
    <div class="max-w-4xl mx-auto px-6 text-center">
      <h1 class="text-5xl font-bold text-gray-900 mb-6">Get In Touch</h1>
      <p class="text-xl text-gray-600 mb-16">
        Ready to start your project? We'd love to hear from you.
      </p>
      
      <div class="bg-white p-8 rounded-2xl border border-gray-100 max-w-md mx-auto">
        <form class="space-y-6">
          <input type="text" placeholder="Your Name" class="w-full px-4 py-3 border border-gray-300 rounded-lg">
          <input type="email" placeholder="Your Email" class="w-full px-4 py-3 border border-gray-300 rounded-lg">
          <textarea placeholder="Tell us about your project..." rows="4" class="w-full px-4 py-3 border border-gray-300 rounded-lg"></textarea>
          <button class="w-full bg-gray-900 text-white py-3 px-6 rounded-lg font-semibold hover:bg-gray-800 transition-colors">
            Send Message
          </button>
        </form>
      </div>
    </div>
  </div>
</template>

<script setup>
useSeoMeta({
  title: 'Contact Us - YourCompany',
  description: 'Get in touch with us to discuss your next digital project.',
})
</script>
