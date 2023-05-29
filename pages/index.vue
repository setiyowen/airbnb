<template>
  <div>
    <div class="bg-[url('/img/bg.png')] bg-fixed bg-cover h-screen">
      <div>
        <div class="flex">
          <div class="pl-[25.65px] pt-[15.61px]">
            <img src="/img/logoairbnb.png" class="w-[34px] h-[34px]" />
          </div>
          <div class="flex gap-5 text-white absolute top-[27px] right-[24px]">
            <NuxtLink to="/about" class="gap-2.5">Français (FR)</NuxtLink>
            <NuxtLink to="/about" class="gap-3">EUR €</NuxtLink>
            <NuxtLink to="/about" class="gap-3">Devenir hôte</NuxtLink>
            <NuxtLink to="/about" class="gap-3">Créer son expérience</NuxtLink>
            <NuxtLink to="/about" class="gap-3">Aide</NuxtLink>
            <NuxtLink to="/about" class="gap-3">Inscription</NuxtLink>
            <NuxtLink to="/about" class="gap-3">Connexion</NuxtLink>
          </div>

          <div
            class="bg-white w-[391px] h-[508px] mt-[132px] ml-[80px] rounded-md"
          >
            <div class="px-[24px] pt-[32px] text-2xl">
              <p class="text-gray-600 font-semibold">
                Réservez des hébergements et des activités uniques.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>

    <explor />

    <Heber />

    <deco />

    <loge />
  </div>
</template>
