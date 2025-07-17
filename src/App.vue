<script setup lang="ts">
import Header from "./components/Header.vue";
</script>

<template>
  <div class="min-h-screen flex flex-col font-sans bg-red-500">
    <!-- Header -->
    <Header />

    <!-- Hero Section -->
    <section class="flex-1 bg-gray-100 py-20 text-center px-4">
      <h2 class="text-4xl font-extrabold mb-4">
        Fast & Modern with Vite + Vue
      </h2>
      <p class="text-lg text-gray-600 mb-8">
        Build blazing-fast apps with the best DX.
      </p>
      <button
        class="bg-blue-600 text-white px-6 py-3 rounded-lg hover:bg-blue-700 transition"
      >
        Get Started
      </button>
    </section>

    <!-- Features -->
    <section id="features" class="py-20 bg-white">
      <div class="container mx-auto grid md:grid-cols-3 gap-6 px-4">
        <div class="p-6 border rounded-lg shadow">
          <h3 class="text-xl font-semibold mb-2">💡 Easy to Use</h3>
          <p>Get started quickly with minimal config.</p>
        </div>
        <div class="p-6 border rounded-lg shadow">
          <h3 class="text-xl font-semibold mb-2">⚡ Super Fast</h3>
          <p>Vite’s lightning-fast HMR makes development smooth.</p>
        </div>
        <div class="p-6 border rounded-lg shadow">
          <h3 class="text-xl font-semibold mb-2">🎨 Modern Stack</h3>
          <p>Works perfectly with Vue 3 & TailwindCSS.</p>
        </div>
      </div>
    </section>

    <!-- Contact -->
    <section id="contact" class="bg-gray-100 py-20 text-center">
      <h2 class="text-3xl font-bold mb-4">Let’s Connect</h2>
      <p class="mb-2">📧 hello@example.com</p>
      <p>📞 +123 456 7890</p>
    </section>

    <!-- Footer -->
    <footer class="bg-blue-600 text-white text-center p-4">
      © 2025 Your Brand. All rights reserved.
    </footer>
  </div>
</template>

<style>
body {
  margin: 0;
  font-family: sans-serif;
}
</style>
