<template>
  <div class="text-center mt-10">
    <h2 class="text-2xl font-semibold">Доступные сервисы</h2>
    <ul class="flex justify-center gap-5 mt-5">
      <li>
        <NuxtImg
          src="http://localhost:3000/youtube.png"
          :width="50"
          :height="50"
        />
      </li>
      <li>
        <NuxtImg
          src="http://localhost:3000/spotify.png"
          :width="50"
          :height="50"
        />
      </li>
      <li>
        <NuxtImg
          src="http://localhost:3000/soundcloud.png"
          :width="50"
          :height="50"
        />
      </li>
      <li>
        <NuxtImg
          src="http://localhost:3000/yandex-music.png"
          :width="50"
          :height="50"
        />
      </li>
      <li>
        <NuxtImg src="http://localhost:3000/vk.png" :width="50" :height="50" />
      </li>
    </ul>
  </div>
</template>
