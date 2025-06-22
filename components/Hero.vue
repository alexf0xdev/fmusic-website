<template>
  <div class="text-center mt-32">
    <h1 class="text-4xl md:text-5xl lg:text-6xl font-semibold">
      Музыкальный Discord-бот
    </h1>
    <p class="sm:text-2xl mt-7">
      Простой, бесплатный и с
      <NuxtLink
        class="text-orange-500"
        to="https://github.com/alexf0xdev/fmusic-discord-bot"
        target="_blank"
      >
        открытым исходным кодом</NuxtLink
      >.
    </p>
    <div class="flex flex-col sm:flex-row sm:justify-center gap-2 mt-10">
      <NuxtLink
        class="flex items-center justify-center gap-2 bg-orange-500 px-7 py-3 text-xl rounded"
        to="https://discord.com/oauth2/authorize?client_id=1373747179319202015"
        target="_blank"
      >
        <Icon name="fa6-brands:discord" />
        Добавить на сервер
      </NuxtLink>
      <NuxtLink
        class="flex items-center justify-center gap-2 bg-neutral-800 px-5 py-2.5 rounded"
        to="/commands"
      >
        <Icon class="text-2xl" name="tabler:command" />
        Список команд
      </NuxtLink>
    </div>
  </div>
</template>
