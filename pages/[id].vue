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
                <div>
                    <p class="p-10 ml-40">Detail Products</p>
                </div>
            </div>
            <div class="flex flex-col ml-240 mb-[10px] gap-4">
                <img src="/img/ip1.jpg" class="w-[300px] ml-40 rounded-lg">
                <div class="flex gap-3 ml-40 rounded-xl hover:">
                    <img src="/img/ip2.jpg"
                        class="w-[90px] rounded-lg max-w-xs transition duration-300 ease-in-out hover:scale-110">
                    <img src="/img/ip3.jpg"
                        class="w-[90px] rounded-lg max-w-xs transition duration-300 ease-in-out hover:scale-110">
                    <img src="/img/ip4.jpg"
                        class="w-[90px] rounded-lg max-w-xs transition duration-300 ease-in-out hover:scale-110">
                </div>
            </div>
            <!-- <h1 class="font-medium text-3xl ml-[80px] mt-[20px]">{{ product.title }}</h1> -->
            <!-- details -->
            <!-- <div class="ml-[80px] w-[700px]">
                        <div class="flex justify-between items-center">
                            <div class="">
                                <p class="font-base text-2xl">{{ product.title }}</p>
                                <p class="pb-[10px] ">{{ product.brand }} . {{ product.category }}</p>
                            </div>
                            <div class="">
                                <div class="bg-[url('/img/lego1.png')] bg-cover w-[40px] h-[40px] rounded-full"> -->
            <!-- <div class="">
                                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-5 h-5 ml-[30px] top-[10px]">
                                            <path fill-rule="evenodd" d="M7.5 6a4.5 4.5 0 119 0 4.5 4.5 0 01-9 0zM3.751 20.105a8.25 8.25 0 0116.498 0 .75.75 0 01-.437.695A18.683 18.683 0 0112 22.5c-2.786 0-5.433-.608-7.812-1.7a.75.75 0 01-.437-.695z" clip-rule="evenodd" />
                                        </svg>
                            </div> -->

        </div>
        <div class="mt-[150px] ml-7">
            <p class="flex-col text-xl  mb-10 text-gray-700">(IBOX) Apple iPhone 14 Pro Max ProMax <br>1TB 512GB 256GB 128GB
                Resmi TAM
                -
                128GB, </p>
            <ul class="list-disc ml-[10px] mt-[10px] text-gray-800">
                <li> Positif review 99 % dr 100 % kepuasan customer</li>
                <li>Sudah melayani 100,000++ customer secara online</li>
                <li>Garansi Resmi Apple 1 Tahun </li>
                <li>Brand new - Original - Segel</li>
                <li>Layar : 6.7 inch</li>
                <li>Ukuran : 128GB - 256GB - 512GB - 1TB</li>
                <li>BNIB (Brand New In Box)</li>
                <li>Imei terdaftar di kemenperin</li>
                <li>Mohon membaca catatan toko sebelum membeli</li>
            </ul>
        </div>
        <div class="border-2 p-2 ml-10 w-[290px] h-[300px] rounded-lg border-gray-500 shadow-xl mt-40">
            <!-- header card -->
            <div class="flex items-center justify-between py-5 ml-[24px] mr-[10px]">
                <div class="flex-none gap-[3px] items-center">
                    <p class="font-medium text-xl text-black ">Atur jumlah dan catatan</p>
                    <div class="custom-number-input h-10 w-32 rounded-xl">
                        <div class="flex flex-row h-8 w-full  relative bg-transparent mt-5">
                            <button data-action="decrement"
                                class=" bg-gray-300 text-gray-600 hover:text-gray-700 hover:bg-gray-400 h-full w-20 rounded-l cursor-pointer outline-none">
                                <span class="m-auto text-2xl font-thin">−</span>
                            </button>
                            <input type="number"
                                class="text-center w-full bg-gray-300 font-semibold text-md hover:text-black focus:text-black flex items-center text-gray-700  outline-none"
                                name="custom-input-number" value="0">
                            <button data-action="increment"
                                class="bg-gray-300 text-gray-600 hover:text-gray-700 hover:bg-gray-400 h-full w-20 rounded-r cursor-pointer">
                                <span class="m-auto text-2xl font-thin">+</span>
                            </button>

                        </div>
                        <!-- stok total -->
                        <!-- <div class="flex items-center justify-center align">
                            <p>Stok :</p>
                        </div> -->
                    </div>
                    <!-- subtotal -->
                    <div class="flex gap-[110px] mt-5">
                        <p class="font-base">Subtotal</p>
                        <p class="text-xl font-bold">${{ product.total }}</p>
                    </div>
                    <div>
                        <NuxtLink :to="`/checkout/` + id" :key="product.id">
                            <div
                                class="p-2 bg-gray-700 mx-5 ml-[10px] mt-[20px] rounded-md justify-center content-center hover:bg-gray-600">
                                <p class="text-center font-semibold text-white">+ Keranjang</p>
                            </div>
                        </NuxtLink>
                        <NuxtLink :to="'/beli/' + id" :key="product.id">
                            <div class="p-1 mx-5 ml-[10px] mt-[10px] rounded-md justify-center content-center border-2">
                                <p class="text-center font-semibold text-white">Beli Langsung</p>
                            </div>
                        </NuxtLink>
                    </div>
                </div>
            </div>
        </div>

    </div>
    <!-- </div>
    </div>
</div> -->
</template>
<!-- items -->
<!-- <div v-for="product in data.products" :key="product.id">
            {{ product.title }}
            {{ product.description }}
            {{ product.price }}
        </div> -->
<!-- <style>
input[type='number']::-webkit-inner-spin-button,
input[type='number']::-webkit-outer-spin-button {
    -webkit-appearance: none;
    margin: 0;
}

.custom-number-input input:focus {
    outline: none !important;
}

.custom-number-input button:focus {
    outline: none !important;
}
</style> -->


<script setup>

const { id } = useRoute().params
const url = 'https://dummyjson.com/products/' + id

// fetch
const { data: data } = await useFetch(url)
const { data: product } = await useFetch('https://dummyjson.com/products')



</script>

