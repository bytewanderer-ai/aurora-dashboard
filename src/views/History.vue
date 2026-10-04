<template>
  <div class="container narrow">
    <section class="page-heading">
      <p class="eyebrow">PROJECT HISTORY</p>
      <h1>Development timeline</h1>
      <p class="lead">
        A short record of the Aurora Dashboard migration.
      </p>
    </section>

    <section class="timeline">
      <article v-for="item in timeline" :key="item.year" class="timeline-item">
        <div class="year">{{ item.year }}</div>
        <div>
          <h2>{{ item.title }}</h2>
          <p>{{ item.description }}</p>
        </div>
      </article>
    </section>

    <section class="note">
      <strong>Historical note</strong>
      <p>
        Some records from the 2019 migration were preserved outside the current
        repository.
      </p>
    </section>
  </div>
</template>

<script setup>
const timeline = [
  {
    year: '2018',
    title: 'Initial prototype',
    description: 'The first internal dashboard was assembled for archive monitoring.'
  },
  {
    year: '2019',
    title: 'Migration preparation',
    description: 'Legacy records were reviewed before the system moved to a new environment.'
  },
  {
    year: '2020',
    title: 'Public dashboard',
    description: 'A simplified version was published for project reference.'
  },
  {
    year: '2021',
    title: 'Archive cleanup',
    description: 'Obsolete components were removed from the active project.'
  }
]
</script>