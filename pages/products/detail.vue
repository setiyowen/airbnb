<template>
    <div class="flex border-b-2 h-[81px] items-center justify-between sticky top-0 bg-white">
        <img src="/img/airbnbpinklogo.png" class="h-[81px] w-auto items-center">

        <!-- fitur search -->
        <div class="rounded-3xl border-2 justify-between items-center px-3 py-2">
            <input class="outline-none gap-2" type="search" name="search" id="search">
            <button class="bg-pink-600 p-2 text-white rounded-2xl" type="submit"><svg xmlns="http://www.w3.org/2000/svg"
                    fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-3 h-3">
                    <path stroke-linecap="round" stroke-linejoin="round"
                        d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
                </svg>
            </button>

        </div>
        <div class="flex gap-2 items-center pr-[10px]">
            <p class="font-bold">Become a Host</p>
            <img src="/img/globe.png" class="h-[16px] w[16px]">
            <div class="w-[81px] h-[38px] rounded-3xl border-2">

            </div>
        </div>
    </div>
    <!-- list produk category -->
    <div class="flex justify-center">
        <Category />
    </div>


    <div
        class="grid lg:grid-cols-4 md:grid-cols-3 sm:grid-cols-2 xs:grid-cols-1 ml-[80px] mr-[80px] mt-[50px] gap-[8px] overflow-hidden">
        <div class="" v-for="items in product.products" :key="items.id">
            <NuxtLink :to="`${items.id}`">
                <div>
                    <div>
                        <img :src="items.thumbnail" class="w-auto h-[240px]  rounded-md">
                    </div>
                    <div>
                        <p class="text-[16px] p-[1px] text-gray-600 font-bold mt-1">{{ items.title }}</p>
                        <p class="text-[10px] text-px-[3px] text-justify">${{ items.description }}</p>
                        <p class="text-[14px] text-start text-gray-600 font-bold">${{ items.price }}</p>
                    </div>
                </div>
            </NuxtLink>

        </div>
        <div v-for="product in data.products" :key="product.id">
            {{ product.title }}
            {{ product.description }}
            {{ product.price }}
        </div>
    </div>
</template>

<script setup>
const { data: product } = await useFetch('https://dummyjson.com/products')
// const { data: cat } = await useFetch('https://dummyjson.com/products/categories')



</script>