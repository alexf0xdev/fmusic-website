<script setup lang="ts">
import type { NuxtError } from '#app'

const props = defineProps({
  error: Object as () => NuxtError,
})

useSeoMeta({ title: props.error?.statusCode })

const handleError = () => clearError({ redirect: '/' })
</script>

<template>
  <NuxtLayout>
    <div class="flex items-center justify-center min-h-[calc(100vh-172px)]">
      <div class="text-center w-full">
        <h1 class="text-7xl font-semibold">{{ error?.statusCode }}</h1>
        <p class="mt-5" v-if="error?.statusCode === 404">
          Страница не найдена или удалена
        </p>
        <p class="mt-5" v-else>Неизвестная ошибка</p>
        <div class="flex flex-col sm:flex-row sm:justify-center mt-5">
          <button
            class="flex items-center justify-center gap-2 bg-orange-500 px-5 py-2.5 rounded cursor-pointer"
            @click="handleError"
          >
            <Icon class="text-2xl" name="tabler:home" />
            На главную
          </button>
        </div>
      </div>
    </div>
  </NuxtLayout>
</template>
