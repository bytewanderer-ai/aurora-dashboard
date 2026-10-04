<template>
  <header class="navbar">
    <div class="container nav-inner">
      <RouterLink to="/" class="brand">
        <span class="brand-mark">A</span>
        <span>
          <strong>Aurora</strong>
          <small>Dashboard</small>
        </span>
      </RouterLink>

      <nav>
        <RouterLink to="/">Overview</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>
</template>