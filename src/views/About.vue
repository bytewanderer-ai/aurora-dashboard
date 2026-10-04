<template>
  <div class="container narrow">
    <section class="page-heading">
      <p class="eyebrow">ABOUT</p>
      <h1>A small project with a long history.</h1>
    </section>

    <AboutCard />

    <section class="panel">
      <h2>Technology</h2>
      <div class="tags">
        <span>Vue 3</span>
        <span>Vue Router</span>
        <span>Vite</span>
        <span>JSON</span>
      </div>
    </section>
  </div>
</template>

<script setup>
import AboutCard from '../components/About.vue'
</script>