<template>
  <div>
    <div class="bg-[url('/img/bg.png')] bg-fixed bg-cover h-screen">
      <div>
        <div class="flex">
          <div class="pl-[25.65px] pt-[15.61px]">
            <a href="/" class="flex-shrink-0">
              <img src="/img/logoairbnb.png" class="w-[34px] h-[34px]" />
            </a>
          </div>
          <div class="flex gap-5 text-white absolute top-[27px] right-[24px]">
            <NuxtLink to="https://www.tiket.com" class="gap-3">Français (FR)</NuxtLink>
            <NuxtLink to="https://www.airbnb.com" class="gap-3">EUR €</NuxtLink>
            <NuxtLink to="/about" class="gap-3">Devenir hôte</NuxtLink>
            <NuxtLink to="/products" class="gap-3">Créer son expérience</NuxtLink>
            <NuxtLink to="/airbnb" class="gap-3">Aide</NuxtLink>
            <NuxtLink to="https://www.expedia.co.id/" class="gap-3">Inscription</NuxtLink>
            <NuxtLink to="https://www.pegipegi.com/hotel" class="gap-3">Connexion</NuxtLink>
          </div>

          <div class="bg-white w-[391px] h-[508px] mt-[132px] ml-[80px] rounded-md">
            <div class="px-[24px] pt-[32px] text-2xl">
              <p class="text-gray-600 font-semibold">
                Réservez des hébergements et des activités uniques.
              </p>
            </div>
            <div class="w-[343px]">
              <form class="ml-10 mt-[24px]">
                <div class="mb-6">
                  <label for="Où" class="block mb-2 text-sm font-medium text-gray-900 dark:text-white">Où</label>
                  <input type="search" id="search"
                    class="bg-gray-50 border text-sm rounded-md block w-full p-2.5 dark:placeholder-gray-400"
                    placeholder="Partout" required />
                </div>
                <div class="grid md:grid-cols-2">
                  <div class="relative z-0 w-full ">
                    <label for="text" class="mb-2 text-sm font-medium text-gray-900 dark:text-white">Arrivée</label>
                    <input type="text" id="Arrivée"
                      class="bg-gray-50 border text-sm rounded-md block w-full p-2.5 dark:placeholder-gray-400"
                      placeholder="jj/mm/aaaa" />
                  </div>
                  <div class="relative z-0 w-full">
                    <label for="text" class="mb-2 text-sm font-medium text-gray-900 dark:text-white">Départ</label>
                    <input type="text" id="Arrivée"
                      class="bg-gray-50 border text-sm rounded-md block w-full p-2.5 dark:placeholder-gray-400"
                      placeholder="jj/mm/aaaa" />
                  </div>
                </div>
                <div class="mt-[24px]">
                  <label for="text" class="mb-2 text-sm font-medium">Voyageurs</label>
                  <input type="text"
                    class="bg-gray-50 border text-sm w-full rounded-md block  p-2.5 dark:placeholder-gray-400"
                    placeholder="jj/mm/aaaa" />
                </div>
                <div class="px-[205px] py-9 flex justify-between ">
                  <button type="button" class=" text-white bg-rose-500 p-2.5 rounded-md  mr-[80px]">Rechercher</button>
                </div>
              </form>
            </div>
          </div>
        </div>
      </div>
    </div>

    <explor />

    <Heber />

    <loge />
  </div>
</template>
