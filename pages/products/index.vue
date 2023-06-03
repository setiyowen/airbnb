<template>
    <div>
        <h1>Product List</h1>
        <ul>
            <li v-for="product in products" :key="product.id">
                <router-link :to="`/product/detail/${product.id}`">{{ product.name }}</router-link>
            </li>
        </ul>
    </div>
</template>
  
<script setup>
import { ref } from 'vue';
import { useFetch } from 'vue-fetch-hooks';

const { data: products } = useFetch('https://dummyjson.com/products');
</script>
  