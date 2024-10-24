<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <ThreeColumnLayout>
    <h2 class="text-3xl font-bold mb-4">Homepage content</h2>
    <ArticleCard v-for="article in articles" :article="article" />

    <template #aside>
      <WidgetFriendSuggestions />
    </template>
  </ThreeColumnLayout>
</template>

