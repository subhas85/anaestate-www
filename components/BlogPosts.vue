<template>
  <section class="blog-posts py-12 bg-white">
    <div class="container mx-auto px-4">
      <h2 class="text-3xl font-bold text-center mb-8">Explore the World of Olive Oil</h2>
      <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-8">
        <div class="blog-post" v-for="item in posts" :key="item.id">
          <img :src="`/images/${item.image}`" alt="" class="blog-post__image mb-4 rounded shadow" />
          <div class="blog-post__content">
            <h3 class="text-xl font-bold mb-2">{{ item.title }}</h3>
            <p class="text-base text-gray-600">{{ item.excerpt }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      posts: [
        {
          id: 1,
          title: "Unlocking the Hidden Flavors: A Guide to EVOO Pairing",
          image: "blog.jpeg",
          slug: "guide-to-evoo-pairing",
          excerpt: "Learn how to pair different EVOOs with your meals to maximize their flavor profile.",
        },
        // Add more blog posts here
      ],
    };
  },
};
</script>

<style scoped>
.blog-posts {
  @apply bg-white;
}

.blog-post__image {
  @apply w-full h-64 object-cover;
}

.blog-post__content {
  @apply p-4 bg-white rounded shadow;
}
</style>