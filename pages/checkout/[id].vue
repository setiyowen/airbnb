<template>
    <div>
        <p>tes</p>
        <!-- <p>{{ product.title }}</p>
        <div></div> class="flex shadow-md my-10">
        <div class="w-3/4 bg-white px-10 py-10">
            <div class="flex justify-between border-b pb-8">
                <h1 class="font-semibold text-2xl">{{ product.title }}</h1>
                <h2 class="font-semibold text-2xl">3 Items</h2>
            </div>
        </div> -->
    </div>
</template>

<script setup>

const { checkout } = useRoute().params
const uri = 'https://dummyjson.com/products/' + id

// fetch
const { data: data } = await useFetch(uri)
const { data: product } = await useFetch('https://dummyjson.com/products')

</script>