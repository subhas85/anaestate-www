<template>
  <section class="reviews py-12 bg-gray-100">
    <div class="container mx-auto px-4">
      <h2 class="text-3xl font-bold text-center mb-8">What Our Customers Are Saying</h2>
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <div class="testimonial p-6 bg-white rounded shadow" v-for="review in reviews" :key="review.id">
          <p class="text-gray-600 italic mb-4">"{{ review.text }}"</p>
          <h3 class="text-xl font-bold text-blue-500">{{ review.name }}</h3>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      reviews: [
        {
          id: 1,
          name: "John Doe",
          text: "This olive oil is incredible! It has a delicious flavor that elevates all my dishes. I highly recommend it!",
        },
        {
          id: 2,
          name: "Jane Smith",
          text: "I've been using Ana's Estate EVOO for years and it's always top-notch. The quality is unmatched and the price is fair. A must-have for any kitchen!",
        },
      ],
    };
  },
};
</script>

<style scoped>
.reviews {
  @apply bg-gray-100;
}

.testimonial {
  @apply p-6 bg-white rounded shadow;
}

.testimonial h3 {
  @apply text-xl font-bold text-blue-500;
}

.testimonial p {
  @apply text-gray-600 italic mb-4;
}
</style>