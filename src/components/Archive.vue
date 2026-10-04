<template>
  <section class="panel">
    <div class="panel-heading">
      <div>
        <p class="eyebrow">ARCHIVE</p>
        <h2>Recent records</h2>
      </div>
      <span class="badge">READ ONLY</span>
    </div>

    <div class="record-list">
      <article v-for="record in records" :key="record.id" class="record">
        <div class="record-id">{{ record.id }}</div>
        <div class="record-main">
          <h3>{{ record.name }}</h3>
          <p>{{ record.year }} · {{ record.status }}</p>
        </div>
      </article>
    </div>
  </section>
</template>

<script setup>
defineProps({
  records: {
    type: Array,
    required: true
  }
})
</script>