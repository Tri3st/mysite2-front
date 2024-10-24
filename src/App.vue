<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
      <h1 class="text-3xl text-emerald-800 text-center">Hello</h1>

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/posts"></RouterLink>
      </nav>
  </header>

  <RouterView />
</template>

