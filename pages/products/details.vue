<template>
    <div>
        <h1>Product Detail</h1>
        <p>ID: {{ id }}</p>
        <p>Name: {{ product.name }}</p>
        <p>Description: {{ product.description }}</p>
        <p>Price: {{ product.price }}</p>
    </div>
</template>
  
<script setup>
import { ref } from 'vue';
import { useRoute } from 'vue-router';
import { useFetch } from 'vue-fetch-hooks';

const { id } = useRoute().params;
const { data: product } = useFetch(`https://dummyjson.com/products/${id}`);
</script>
  