<template>
    <div>
        <p>product details for {{ id }}</p>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Fugiat aperiam eveniet dolorum nobis vel odio eos qui
            dicta excepturi sit repellat illum provident, eaque alias aliquid autem? Reiciendis, incidunt neque!</p>
    </div>
</template>

<script setup>
const { id } = useRouter().params
</script>

<style scoped></style>