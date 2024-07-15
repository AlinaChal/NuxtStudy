<template>
    <div>
        <div class="grid grid-cols-4 gap-5">
            <div v-for = "p in products">
                <ProductCard :product="p" />
            </div>
        </div>
    </div>
</template>

<script setup>

//fethc the products
const {data: products} = await useFetch('https://fakestoreapi.com/products')

definePageMeta({
    layout: 'products' 
})

useHead ({
    title: 'First project | Catalog',
    meta: [
        { name: 'description', content: 'Nuxt 3 catalog'}
    ]
})
</script>


<style scoped>

</style>
