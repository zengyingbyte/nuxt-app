<template>
  <div>
    <div class="grid grid-cols-4 gap-5">
      <div v-for="(p, i) in products" :key="i">
        <ProductCard :product="p" />
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
definePageMeta({
  layout: "products",
});

// fetch the products
const { data: products } = await useFetch("https://fakestoreapi.com/products");

useHead({
  title: "Nuxt App | Merch",
  meta: [{ name: "description", content: "Nuxt 3 Merch" }],
});
</script>

<style scoped>
</style>