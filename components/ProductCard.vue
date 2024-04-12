<template>
  <div class="product-card rounded overflow-hidden shadow-lg">
    <img :src="`/images/product/${product.image}`" alt="" class="product-card__image w-full" />
    <div class="px-6 py-4">
      <div class="font-bold text-xl mb-2">{{ product.name }}</div>
      <p class="text-gray-700 text-base">{{ product.description }}</p>
    </div>
    <div class="px-6 pt-4 pb-2">
      <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">${{ product.price }}</span>
      <nuxt-link to="/cart" class="btn btn-primary mt-4 inline-block bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">Add to Cart</nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    product: Object,
  },
};
</script>

<style scoped>
.product-card {
  @apply bg-white rounded shadow-md;
}

.product-card__image {
  @apply w-full h-48 object-cover;
}
</style>