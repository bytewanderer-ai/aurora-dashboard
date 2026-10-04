<template>
  <div>
    <section class="hero container">
      <div>
        <p class="eyebrow">AURORA SYSTEMS</p>
        <h1>Archive monitoring,<br /><span>kept simple.</span></h1>
        <p class="lead">
          A lightweight dashboard for tracking historical project records,
          migration status, and archived components.
        </p>
      </div>

      <div class="status-card">
        <span class="status-dot"></span>
        <div>
          <strong>Archive status</strong>
          <p>Operational · Read only</p>
        </div>
      </div>
    </section>

    <section class="container stats">
      <div class="stat">
        <span>PROJECTS</span>
        <strong>03</strong>
      </div>
      <div class="stat">
        <span>ARCHIVED</span>
        <strong>02</strong>
      </div>
      <div class="stat">
        <span>LAST UPDATE</span>
        <strong>2021</strong>
      </div>
    </section>

    <div class="container">
      <Archive :records="records" />
    </div>
  </div>
</template>

<script setup>
import { onMounted, ref } from 'vue'
import Archive from '../components/Archive.vue'

const records = ref([])

onMounted(async () => {
  const response = await fetch('/archive.json')
  const data = await response.json()
  records.value = data.records
})
</script>