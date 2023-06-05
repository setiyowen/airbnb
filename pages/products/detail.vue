<template>
    <div class="flex border-b-2 h-[81px] items-center justify-between sticky top-0 bg-white">

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
    </div>
</template>

<script setup>
const { data: product } = await useFetch('https://dummyjson.com/products')



</script>