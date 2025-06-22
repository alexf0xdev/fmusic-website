<script setup lang="ts">
useHead({
  titleTemplate: (title) => (title ? `${title} - FMusic` : 'FMusic'),
  meta: [{ name: 'description', content: 'Музыкальный Discord-бот.' }],
})
</script>

<template>
  <NuxtLayout>
    <NuxtPage />
  </NuxtLayout>
</template>
