<template>
  <div class="testimonial">
    <img
      :src="`~/assets/profiles/${review.image}`"
      alt=""
      class="testimonial__image"
    />
    <div class="testimonial__content">
      <p class="text-base mb-4">{{ review.text }}</p>
      <h4 class="text-lg font-bold">{{ review.name }}</h4>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    review: Object, // Define a prop to receive review data
  },
};
</script>

<style scoped>
.testimonial {
  @apply rounded shadow-md p-4 flex items-center;
}

.testimonial__image {
  @apply w-16 h-16 rounded-full mr-4 object-cover;
}

.testimonial__content {
  @apply flex-grow;
}
</style>
