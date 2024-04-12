<template>
  <section class="about-us py-16 bg-gray-100">
    <div class="container mx-auto px-4">
      <h2 class="text-3xl font-bold text-center mb-8">About Ana's Estate</h2>
      <div class="grid md:grid-cols-2 gap-8">
        <div class="about-us__content">
          <p class="text-base mb-4">
            At Ana's Estate, we produce the finest extra virgin olive oil using
            traditional methods.
          </p>
          <p class="text-base mb-4">
            We are committed to sustainable practices that preserve the health
            of our land and ensure the future of our olive trees. Our meticulous
            harvesting and pressing techniques guarantee the exceptional quality
            and unique flavor profile of our EVOO.
          </p>
        </div>
        <div class="about-us__images">
          <img
            src="/assets/images/grandpa.jpeg"
            alt="Ana's Estate Olive Grove"
            class="about-image mb-4 rounded shadow"
          />
          <img
            src="/assets/images/table.jpeg"
            alt="Olive Harvesting"
            class="about-image mb-4 rounded shadow"
          />
          <img
            src="/assets/images/process.jpeg"
            alt="Olive Oil Bottling"
            class="about-image mb-4 rounded shadow"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.about-us {
  @apply py-16 bg-gray-100;
}

.about-us__content {
  @apply text-gray-700;
}

.about-image {
  @apply w-64 h-64 object-cover rounded shadow-md;
}
</style>
