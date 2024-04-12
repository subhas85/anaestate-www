<template>
  <div>
    <div style="text-align: center">
      <NavigationMenu style="display: flex; justify-content: center">
        <NavigationMenuList style="display: flex">
          <NavigationMenuItem>
            <NuxtLink to="/">
              <NavigationMenuLink :class="navigationMenuTriggerStyle()">
                Home
              </NavigationMenuLink>
            </NuxtLink>

            <NuxtLink to="/blog">
              <NavigationMenuLink :class="navigationMenuTriggerStyle()">
                Blog
              </NavigationMenuLink>
            </NuxtLink>
          </NavigationMenuItem>
        </NavigationMenuList>
      </NavigationMenu>
    </div>
    <div>
      <div
        class="hero-section"
        style="
          background-image: url('/images/Olive-trees-grove-Sparta-Greece-Peloponnese_1080x.jpg');
        "
      >
        <div class="hero-content">
          <h1>From our farm to your table.</h1>
          <h2>Ana's Estate Extra Virgin Olive Oil</h2>
          <button class="hero-button">Discover our products</button>
        </div>
      </div>
    </div>
    <About />
    <Products />
    <Reviews />
    <BlogPosts />
    <CtaSection />
    <Footer />
  </div>
</template>
<script lang="ts">
import { navigationMenuTriggerStyle } from "@/components/ui/navigation-menu";
import About from "./components/About.vue";
import Products from "./components/Products.vue";
import Reviews from "./components/Reviews.vue";
import BlogPosts from "./components/BlogPosts.vue";
import CtaSection from "./components/CtaSection.vue";
import Footer from "./components/Footer.vue";

export default {
  components: {
    About,
    Products,
    Reviews,
    BlogPosts,
    CtaSection,
    Footer,
  },

  methods: {
    navigationMenuTriggerStyle,
  },
};
</script>
<style scoped>
.hero-section {
  height: 100vh;
  clear: both;
  background-size: cover;
  background-position: center;
  display: flex;
  justify-content: center;
  align-items: center;
}

.hero-content {
  text-align: center;
  color: white;
}

.hero-button {
  background-color: #ff7f50;
  color: white;
  padding: 10px 20px;
  border: none;
  cursor: pointer;
  text-transform: uppercase;
  margin-top: 20px;
}
</style>
