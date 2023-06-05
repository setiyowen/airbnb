<template>
    <div class="flex border-2 h-[81px] items-center justify-between">
        <img src="/img/logoairbnb.png" class="h-[81px] w-auto items-center">
        <div class="w-[352px] h-[48px] rounded-3xl border-2">

        </div>
    </div>
</template>

<script setup>
const { id } = useRoute().params
const uri = 'https://dummyjson.com/products/' + id

// fetch
const { data: product } = await useFetch(uri)

</script>

<style></style>