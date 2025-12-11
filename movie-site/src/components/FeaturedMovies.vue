
<template>
  <section class="featured-section">
    <div class="featured-container">
      <h2>Featured Movies</h2>
      <div class="featured-scroll">
        <MovieCard v-for="n in 8" :key="n" />
      </div>
    </div>
  </section>
</template>

<script setup>
import MovieCard from './MovieCard.vue'
</script>

<style scoped>
.featured-section {
  background: #111;
  padding: 3.5rem 0 2.5rem 0;
}
.featured-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 3vw;
}
.featured-container h2 {
  color: #fff;
  font-size: 2.2rem;
  font-weight: 800;
  margin-bottom: 2rem;
  letter-spacing: -1px;
}
.featured-scroll {
  display: flex;
  overflow-x: auto;
  gap: 1.5rem;
  padding-bottom: 0.5rem;
  scrollbar-width: thin;
  scrollbar-color: #333 #111;
}
.featured-scroll::-webkit-scrollbar {
  height: 8px;
}
.featured-scroll::-webkit-scrollbar-thumb {
  background: #333;
  border-radius: 4px;
}
.featured-scroll::-webkit-scrollbar-track {
  background: #111;
}
@media (max-width: 700px) {
  .featured-container h2 {
    font-size: 1.3rem;
  }
  .featured-section {
    padding: 2rem 0 1.2rem 0;
  }
}
</style>
