<template>
  <section class="cta">
    <div class="container mx-auto px-4 py-16 flex flex-col items-center justify-center text-center">
      <h2 class="text-2xl font-bold mb-4">Discover the Taste of Authentic EVOO</h2>
      <p class="mb-8">Experience the rich, fruity flavors of Ana's Estate EVOO. Perfect for cooking, dipping, and dressing.</p>
      <nuxt-link to="/shop" class="btn btn-primary btn-lg">Shop Ana's Estate EVOO Now</nuxt-link>
    </div>
  </section>
</template>

<style scoped>
.cta {
  @apply bg-gray-200;
}

.btn {
  @apply py-2 px-4 bg-blue-500 text-white font-semibold rounded-lg shadow-md hover:bg-blue-700 focus:outline-none focus:ring-2 focus:ring-blue-400 focus:ring-opacity-75;
}
</style>