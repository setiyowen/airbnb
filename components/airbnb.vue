<template>
    <div class="flex  items-center justify-between sticky top-0 bg-white">
        <div class="flex gap-2 items-center p-[20px] h-[80px]">
            <p class="font-medium mr-10">List Product</p>
        </div>
        <!-- fitur search  -->
        <div class="rounded-lg border-2 justify-between items-center py-1 px-2 mr-12">
            <input class="outline-none gap-2" type="search" id="search" placeholder="Search">
            <button class=" text-gray-500 p-2 mr-1" type="submit">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="3"
                    stroke="currentColor" class="w-4 h-4">
                    <path stroke-linecap="round" stroke-linejoin="round"
                        d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
                </svg>
            </button>
        </div>
    </div>
    <div
        class="grid lg:grid-cols-4 md:grid-cols-3 sm:grid-cols-2 xs:grid-cols-1 ml-[80px] mr-[80px] mt-[50px] gap-[8px] overflow-hidden">
        <div class="" v-for="items in product.products" :key="items.id">
            <NuxtLink :to="`/${items.id}`">
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
        <detail />
    </div>
</template>

<script setup>
const { data: product } = await useFetch('https://dummyjson.com/products')



</script>

