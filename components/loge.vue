<template>
  <div class="overflow-hidden">
    <div>
      <p class="text-xl font-semibold p-20 mt-72">
        Logements dans le monde entier
      </p>
    </div>

    <div
      class="grid lg:grid-cols-4 md:grid-cols-2 sm:grid-cols-1 ml-[80px] mr-[80px] gap-[8px]">
      <div class="flex-none">
        <img src="/img/loge1.png" class="w-[290px] h-[200px] rounded-md" />
        <div class="flex">
          <p class="text-base border-[1px] border-black m-2">SUPERHOST</p>
          <p
            class="text-base text-gray-500 items-center pl-[13px] mt-[10px] w-[120px]">
            Toledo
          </p>
          <div class="flex"></div>
        </div>
        <p class="text-sm text-slate-900 mt-[8px]">
          À partir de 577€/personne - 3 jours
        </p>
      </div>
      <div>
        <img src="/img/loge2.png" class="w-[290px] h-[200] rounded-md" />
        <div class="flex">
          <p class="text-base border-[1px] m-2 border-black">SUPERHOST</p>
          <p
            class="text-base text-gray-500 items-center pl-[13px] mt-[10px] w-[120px]">
            Mesa
          </p>
        </div>
        <p class="text-sm text-slate-900 mt-[8px]">
          À partir de 577€/personne - 3 jours
        </p>
      </div>
      <div class="">
        <img src="/img/loge3.png" class="w-[290px] h-[200] rounded" />
        <div class="flex">
          <p class="text-base border-[1px] m-2 border-black">SUPERHOST</p>
          <p
            class="text-base text-gray-500 items-center pl-[13px] mt-[10px] w-[120px]">
            Utica
          </p>
        </div>
        <p class="text-sm text-slate-900 mt-[8px]">
          À partir de 577€/personne - 3 jours
        </p>
      </div>
      <div class="">
        <img src="/img/loge4.png" class="w-[290px] h-[200] rounded" />
        <div class="flex">
          <p class="text-base border-[1px] m-2 border-black">SUPERHOST</p>
          <p
            class="text-base text-gray-500 items-center pl-[13px] mt-[10px] w-[120px]">
            South Bend
          </p>
        </div>
        <p class="text-sm text-slate-900 mt-[8px]">
          À partir de 577€/personne - 3 jours
        </p>
      </div>
      <div class="">
        <img src="/img/loge5.png" class="w-[290px] h-[200] rounded" />
        <div class="flex">
          <p class="text-base border-[1px] m-2 border-black">SUPERHOST</p>
          <p
            class="text-base text-gray-500 items-center pl-[13px] mt-[10px] w-[120px]">
            South Bend
          </p>
        </div>
        <p class="text-sm text-slate-900 mt-[8px]">
          À partir de 577€/personne - 3 jours
        </p>
      </div>
      <div class="">
        <img src="/img/loge6.png" class="w-[290px] h-[200] rounded" />
        <div class="flex">
          <p class="text-base border-[1px] m-2 border-black">SUPERHOST</p>
          <p
            class="text-base text-gray-500 items-center pl-[13px] mt-[10px] w-[120px]">
            South Bend
          </p>
        </div>
        <p class="text-sm text-slate-900 mt-[8px]">
          À partir de 577€/personne - 3 jours
        </p>
      </div>
      <div class="">
        <img src="/img/loge7.png" class="w-[290px] h-[200] rounded" />
        <div class="flex">
          <p class="text-base border-[1px] m-2 border-black">SUPERHOST</p>
          <p
            class="text-base text-gray-500 items-center pl-[13px] mt-[10px] w-[120px]">
            South Bend
          </p>
        </div>
        <div>
          <p class="text-sm text-slate-900 mt-[8px]">
            À partir de 577€/personne - 3 jours
          </p>
        </div>
      </div>
      <div class="">
        <img src="/img/loge8.png" class="w-[290px] h-[200] rounded" />
        <div class="flex">
          <p class="text-base border-[1px] m-2 border-black">SUPERHOST</p>
          <p
            class="text-base text-gray-500 items-center pl-[13px] mt-[10px] w-[120px]">
            South Bend
          </p>
        </div>
        <div>
          <p class="text-sm text-slate-900 mt-[8px]">
            À partir de 577€/personne - 3 jours
          </p>
        </div>
      </div>
    </div>
  </div>
  <experiance />
  <destionation />
</template>

<script>
import experiance from "./experiance.vue";
export default {
  components: { experiance },
};
</script>

<style></style>
