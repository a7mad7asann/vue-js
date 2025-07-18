<script setup lang="ts">
import Header from "./components/Header.vue";
import Home from "./pages/Home.vue";
</script>

<template>
  <div class="min-h-screen flex flex-col font-sans ">
    <Header />
    <Home />
  </div>
</template>

<style>
body {
  margin: 0;
  font-family: sans-serif;
}
</style>
