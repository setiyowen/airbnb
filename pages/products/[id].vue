<template>
    <div class="flex border-b-2 h-[81px] items-center justify-between">
        <NuxtLink to="/">
            <img src="/img/logoairbnb.png" class="h-[81px] w-auto items-center">
        </NuxtLink>
        <div class="w-[352px] h-[48px] rounded-3xl border-2">

        </div>
        <div class="flex gap-2 items-center pr-[10px]">
            <p class="font-bold">Become a Host</p>
            <img src="/img/globe.png" class="h-[16px] w[16px]">
            <div class="w-[81px] h-[38px] rounded-3xl border-2">

            </div>
        </div>
    </div>
    <div>

        <div class="bg-white">
            <h1 class="font-medium text-3xl text-[#222222] tracking-wide ml-[80px] mt-[20px]">{{ product.title }}</h1>
            <!-- teks bintang, ulasan, dll -->
            <div class="flex mb-[20px] items-center gap-[10px] ml-[80px]">
                <div class="flex gap-[3px] items-center">
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" class="w-3 h-3">
                        <path fill-rule="evenodd"
                            d="M10.868 2.884c-.321-.772-1.415-.772-1.736 0l-1.83 4.401-4.753.381c-.833.067-1.171 1.107-.536 1.651l3.62 3.102-1.106 4.637c-.194.813.691 1.456 1.405 1.02L10 15.591l4.069 2.485c.713.436 1.598-.207 1.404-1.02l-1.106-4.637 3.62-3.102c.635-.544.297-1.584-.536-1.65l-4.752-.382-1.831-4.401z"
                            clip-rule="evenodd" />
                    </svg>
                    <p class="text-sm font-medium">{{ product.rating }}</p>
                    <p class="text-gray-600 text-sm">(96 ulasan)</p>
                </div>


                <div class="flex gap-[3px] items-center mr-[10px]">
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-3 h-3">
                        <path fill-rule="evenodd"
                            d="M7.5 6a4.5 4.5 0 119 0 4.5 4.5 0 01-9 0zM3.751 20.105a8.25 8.25 0 0116.498 0 .75.75 0 01-.437.695A18.683 18.683 0 0112 22.5c-2.786 0-5.433-.608-7.812-1.7a.75.75 0 01-.437-.695z"
                            clip-rule="evenodd" />
                    </svg>
                    <p class="text-gray-600 text-sm">HostTeladan</p>
                </div>
                <div>
                    <p class="font-semibold underline underline-offset-1">Bandung, Jawa Barat, Indonesia</p>
                </div>
            </div>
        </div>
        <!-- gambar pembuka -->
        <div class="mb-[10px] flex gap-[5px] ">
            <img :src="product.thumbnail" class="w-40% ml-[80px] rounded-l-xl">

            <div class="grid grid-cols-2 gap-[5px] rounded-r-xl">
                <img :src="product.images[1]" class="w-[290px] h-[200px] ">
                <img :src="product.images[2]" class="w-[290px] h-[200px] rounded-tr-xl ">
                <img :src="product.images[3]" class="w-[290px] h-[200px] ">
                <img :src="product.images[3]" class="w-[290px] h-[200px] rounded-br-xl">
            </div>
        </div>

        <!-- flex isi dan card -->
        <div class="flex mt-[100-px] justify-between mr-[100px]">
            <!-- details -->
            <div class="ml-[80px] w-[700px]">
                <div class="flex justify-between items-center">
                    <div class="">
                        <p class="font-base text-2xl">{{ product.title }}</p>
                        <p class="pb-[10px] ">{{ product.brand }} . {{ product.category }}</p>
                    </div>
                    <div class="">
                        <div class="bg-[url('/img/dest2.png')] bg-cover w-[40px] h-[40px] rounded-full">
                            <!-- <div class="">
                                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-5 h-5 ml-[30px] top-[10px]">
                                            <path fill-rule="evenodd" d="M7.5 6a4.5 4.5 0 119 0 4.5 4.5 0 01-9 0zM3.751 20.105a8.25 8.25 0 0116.498 0 .75.75 0 01-.437.695A18.683 18.683 0 0112 22.5c-2.786 0-5.433-.608-7.812-1.7a.75.75 0 01-.437-.695z" clip-rule="evenodd" />
                                        </svg>
                            </div> -->

                        </div>
                    </div>
                </div>
                <div>
                    <!-- isi keterangan host teladan dll -->
                    <div class="pb-[20px] border-b-2">

                        <div class="flex gap-5 items-start mb-[20px]">
                            <!-- pertama -->
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                                stroke="currentColor" class="w-8 h-8">
                                <path stroke-linecap="round" stroke-linejoin="round"
                                    d="M15.75 6a3.75 3.75 0 11-7.5 0 3.75 3.75 0 017.5 0zM4.501 20.118a7.5 7.5 0 0114.998 0A17.933 17.933 0 0112 21.75c-2.676 0-5.216-.584-7.499-1.632z" />
                            </svg>
                            <div>
                                <p class="text-gray-600 font-semibold">
                                    {{ product.description }}
                                </p>
                                <!-- <p class="text-gray-600 overflow-y-visible">HosTeladan adalah tuan rumah berpengalaman dan berpenilaian tinggi yang berkomitmen dalam menyediakan penginapan luar biasa bagi tamu.</p> -->
                            </div>
                        </div>
                    </div>


                </div>

                <!-- card pesan -->
                <div class="border-2 p-2 ml-4 w-[373px] h-[532px] rounded-lg justify-center">
                    <!-- header card -->
                    <div class="flex items-center justify-between py-5 ml-[24px] mr-[10px]">
                        <div class="flex gap-[3px] items-center">
                            <p class="font-medium text-xl text-[#222222] line-through decoration-[1px]">$ {{ product.price
                            }}
                            </p>
                            <p>malam</p>
                            <div class=" bg-pink-600 items-center">
                                <p class="text-center font-bold text-white text-xs px-[3px]">{{ product.discountPercentage
                                }}
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
                            <p
                                class="text-sm font-medium text-gray-600 items-center  ml-[20px] underline underline-offset-1">
                                96
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
                            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor"
                                class="w-5 h-5 mr-[10px]">
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
            </div>


        </div>
    </div>
    <div>
        <!-- ulasan dll -->
    </div>
</template>

<script setup>
const { id } = useRoute().params
const uri = 'https://dummyjson.com/products/' + id

// fetch
const { data: product } = await useFetch(uri)

    // definePageMeta({
    //     layout : 'products'
    // })

</script>
