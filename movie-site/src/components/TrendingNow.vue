<template>
  <section class="trending-section">
    <div class="trending-container">
      <h2>Trending Now</h2>
      <div class="trending-scroll">
        <MovieCard v-for="n in 8" :key="n" />
      </div>
    </div>
  </section>
</template>

<script setup>
import MovieCard from './MovieCard.vue'
</script>

<style scoped>
.trending-section {
  background: #181818;
  padding: 2.5rem 0 2rem 0;
}
.trending-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 3vw;
}
.trending-container h2 {
  color: #fff;
  font-size: 2.1rem;
  font-weight: 800;
  margin-bottom: 1.7rem;
  letter-spacing: -1px;
}
.trending-scroll {
  display: flex;
  overflow-x: auto;
  gap: 1.3rem;
  padding-bottom: 0.5rem;
  scrollbar-width: thin;
  scrollbar-color: #333 #181818;
}
.trending-scroll::-webkit-scrollbar {
  height: 8px;
}
.trending-scroll::-webkit-scrollbar-thumb {
  background: #333;
  border-radius: 4px;
}
.trending-scroll::-webkit-scrollbar-track {
  background: #181818;
}
@media (max-width: 700px) {
  .trending-container h2 {
    font-size: 1.1rem;
  }
  .trending-section {
    padding: 1.2rem 0 1rem 0;
  }
}
</style>
