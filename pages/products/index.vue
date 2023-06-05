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
    <div class="mt-[10px]">
        <!-- deskripsi -->
        <p class="text-xl">Fitur Fitur</p>
        <ul class="list-disc ml-[20px]">
            <li>
                Layar Liquid Retina HD LCD 6,1 inci(1)
            </li>
            <li>Tahan air dan debu (2 meter hingga selama 30 menit, IP68)(1) </li>
            <li>Sistem kamera ganda dengan kamera Ultra Wide dan Wide 12 MP; mode Malam, mode Potret, dan
                video 4K hingga 60 fps </li>
            <li>Kamera depan TrueDepth 12 MP dengan mode Potret, video 4K, dan video gerakan lambat</li>
            <li>Face ID untuk autentikasi aman</li>
            <li>Chip A13 Bionic dengan Neural Engine generasi ketiga</li>
            <li>Kemampuan isi daya cepat</li>
            <li>Pengisian daya nirkabel(4)</li>
            <li>iOS 13 dengan Mode Gelap, alat baru untuk pengeditan foto dan video, dan fitur privasi baru
            </li>
        </ul>
    </div>


    <!-- card pesan -->
    <div class="border-2 p-2 ml-4 w-[373px] h-[532px] rounded-lg justify-center">
        <!-- header card -->
        <div class="flex items-center justify-between py-5 ml-[24px] mr-[10px]">
            <div class="flex gap-[3px] items-center">
                <p class="font-medium text-xl text-[#222222] line-through decoration-[1px]">$ {{ product.price }}
                </p>
                <p>malam</p>
                <div class=" bg-pink-600 items-center">
                    <p class="text-center font-bold text-white text-xs px-[3px]">{{ product.discountPercentage }}
                        off</p>
                </div>
            </div>
            <div class="flex items-center">
                <!-- bintang -->
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" class="w-3 h-3">
                    <path fill-rule="evenodd"
                        d="M10.868 2.884c-.321-.772-1.415-.772-1.736 0l-1.83 4.401-4.753.381c-.833.067-1.171 1.107-.536 1.651l3.62 3.102-1.106 4.637c-.194.813.691 1.456 1.405 1.02L10 15.591l4.069 2.485c.713.436 1.598-.207 1.404-1.02l-1.106-4.637 3.62-3.102c.635-.544.297-1.584-.536-1.65l-4.752-.382-1.831-4.401z"
                        clip-rule="evenodd" />
                </svg>
                <p class="font-semibold items-center">{{ product.rating }}</p>
                <p class="text-sm font-medium text-gray-600 items-center  ml-[20px] underline underline-offset-1">96
                    ulasan</p>
            </div>
        </div>
        <div class="grid grid-cols-2 ml-[24px] text-xs">
            <p class="h-[56px] border-x-2 border-t-2 rounded-tl-md text-xs p-2"><b>Total stok</b> <br> {{
                product.stock }}</p>
            <p class="h-[56px] border-t-2 border-r-2 rounded-tr-md text-xs p-2"><b>CHECK-OUT</b> <br> Tambahkan
                tanggal</p>

            <div class="flex col-span-2 border-2 justify-between items-center rounded-b-md">
                <p class="h-[56px] text-xs p-2"><b>Jumlah</b> <br> 1 Tamu</p>
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" class="w-5 h-5 mr-[10px]">
                    <path fill-rule="evenodd"
                        d="M5.23 7.21a.75.75 0 011.06.02L10 11.168l3.71-3.938a.75.75 0 111.08 1.04l-4.25 4.5a.75.75 0 01-1.08 0l-4.25-4.5a.75.75 0 01.02-1.06z"
                        clip-rule="evenodd" />
                </svg>

            </div>

        </div>
        <NuxtLink to="/checkoutpage">
            <div class="p-2 bg-pink-600 ml-[24px] mt-[10px] rounded-md">
                <p class="text-center font-bold text-white">Pesan</p>
            </div>
        </NuxtLink>

    </div>
    <!-- list produk category -->
    <div class="flex justify-center">
        <!-- <catalog /> -->
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
    </div>
    <slot />
</template>

<script setup>
const { data: product } = await useFetch('https://dummyjson.com/products/1')



</script>

