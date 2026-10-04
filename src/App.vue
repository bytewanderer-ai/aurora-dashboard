<template>
  <div class="app-shell">
    <Navbar />
    <main class="page">
      <RouterView />
    </main>
    <Footer />
  </div>
</template>

<script setup>
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'
</script>