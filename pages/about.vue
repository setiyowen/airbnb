<template>
  <div class="bg-gradient-to-r from-cyan-500 to-blue-500 h-screen">
    <div class="flex">
      <div class="pl-[25.65px] pt-[15.61px]">
        <a href="/" class="flex-shrink-0">
        </a>
      </div>
      <div class="bg-white">
        <h1 class="font-mediun text-3xl  tracking-wide ml-[80px] mt-[20px]">{{ products.title }}</h1>
        <h1>test</h1>
      </div>
    </div>

  </div>
</template>

<script setup>
const { data: product } = await useFetch('https://dummyjson.com/products')



</script>