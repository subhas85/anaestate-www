<template>
  <section class="products">
    <div class="container mx-auto px-4">
      <h2 class="text-3xl font-bold text-center mb-8">
        Discover the Perfect EVOO for You
      </h2>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
        <ProductCard
          v-for="product in products"
          :key="product.id"
          :product="product"
        />
      </div>
    </div>
  </section>
</template>
<script lang="ts">
import ProductCard from "./ProductCard.vue";

export default {
  components: {
    ProductCard,
  },
  data() {
    return {
      products: [
        {
          id: 1,
          name: "Ana's Estate EVOO - 750ml",
          image: "750_shop_360x.png",
          description:
            "Perfect for everyday cooking and drizzling over salads.",
          price: 30.99,
        },
        {
          id: 2,
          name: "Ana's Estate EVOO - 5L",
          image: "750_shop_360x.png",
          description: "A versatile size for all your culinary needs.",
          price: 125.99,
        },
        {
          id: 3,
          name: "Ana's Estate EVOO - 15L",
          image: "750_shop_360x.png",
          description: "Ideal for the home chef and professional kitchen.",
          price: 300.99,
        },
      ],
    };
  },
};
</script>
>
