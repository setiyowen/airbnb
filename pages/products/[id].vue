<template>
    <div>
        div class="grid grid-cols-2 gap-[5px] rounded-r-xl">
        <img :src="product.images[1]" class="w-[290px] h-[200px] ">
        <img :src="product.images[2]" class="w-[290px] h-[200px] rounded-tr-xl ">
        <img :src="product.images[3]" class="w-[290px] h-[200px] ">
        <img :src="product.images[3]" class="w-[290px] h-[200px] rounded-br-xl">
    </div>
</template>

<script setup>
const { id } = useRoute().params
const uri = 'https://dummyjson.com/products/' + id

// fetch
const { data: product } = await useFetch(uri)

</script>
