<template>
    <div class=" flex bg-gradient-to-r from-cyan-500 to-blue-500 h-screen">
        <div class="flex-none ">
            <div class="pl-[25.65px] pt-[15.61px]">
                <a href="/" class="flex-shrink-0">
                    <img src="/img/logoairbnb.png" class="w-[34px] h-[34px]" />
                </a>
                <!-- <div class="rounded-lg border-2 justify-between items-center py-1 px-2 mr-12 flex-none ">
                    <input type="search" id="search" placeholder="Search">
                    <button class=" text-gray-500 p-2 mr-1" type="submit">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="3"
                            stroke="currentColor" class="w-4 h-4">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
                        </svg>
                    </button>

                </div> -->
            </div>
            <p class="p-10">Detail Products</p>
        </div>

        <!-- <div v-for="product in data.products" :key="product.id">
            {{ product.title }}
            {{ product.description }}
            {{ product.price }}
        </div> -->
    </div>
</template>

<script setup>
const { id } = useRoute().params
const url = 'https://dummyjson.com/products/' + id

// fetch
const { data: data } = await useFetch(url)

</script>