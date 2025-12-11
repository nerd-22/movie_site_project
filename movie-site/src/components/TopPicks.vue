<template>
  <section class="toppicks-section">
    <div class="toppicks-container">
      <h2>Top Picks for You</h2>
      <div class="toppicks-scroll">
        <MovieCard v-for="n in 8" :key="n" />
      </div>
    </div>
  </section>
</template>

<script setup>
import MovieCard from './MovieCard.vue'
</script>

<style scoped>
.toppicks-section {
  background: #111;
  padding: 2.5rem 0 2rem 0;
}
.toppicks-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 3vw;
}
.toppicks-container h2 {
  color: #fff;
  font-size: 2.1rem;
  font-weight: 800;
  margin-bottom: 1.7rem;
  letter-spacing: -1px;
}
.toppicks-scroll {
  display: flex;
  overflow-x: auto;
  gap: 1.3rem;
  padding-bottom: 0.5rem;
  scrollbar-width: thin;
  scrollbar-color: #333 #111;
}
.toppicks-scroll::-webkit-scrollbar {
  height: 8px;
}
.toppicks-scroll::-webkit-scrollbar-thumb {
  background: #333;
  border-radius: 4px;
}
.toppicks-scroll::-webkit-scrollbar-track {
  background: #111;
}
@media (max-width: 700px) {
  .toppicks-container h2 {
    font-size: 1.1rem;
  }
  .toppicks-section {
    padding: 1.2rem 0 1rem 0;
  }
}
</style>
