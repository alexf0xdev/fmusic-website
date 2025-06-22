<script setup lang="ts">
const props = defineProps({
  href: String,
})
</script>

<template>
  <NuxtLink class="text-orange-500" :to="href" target="_blank"
    ><slot />
  </NuxtLink>
</template>
