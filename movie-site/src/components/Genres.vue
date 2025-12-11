<template>
  <section class="genres-section">
    <div class="genres-container">
      <h2>Browse by Genre</h2>
      <div class="genres-list">
        <span class="genre">Action</span>
        <span class="genre">Comedy</span>
        <span class="genre">Drama</span>
        <span class="genre">Horror</span>
        <span class="genre">Romance</span>
        <span class="genre">Sci-Fi</span>
        <span class="genre">Documentary</span>
        <span class="genre">Animation</span>
      </div>
    </div>
  </section>
</template>

<script setup>
// Static genres for now
</script>

<style scoped>
.genres-section {
  background: #181818;
  padding: 2.5rem 0 2rem 0;
}
.genres-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 3vw;
}
.genres-container h2 {
  color: #fff;
  font-size: 2.1rem;
  font-weight: 800;
  margin-bottom: 1.7rem;
  letter-spacing: -1px;
}
.genres-list {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
}
.genre {
  background: #232323;
  color: #fff;
  font-weight: 600;
  font-size: 1rem;
  padding: 0.7rem 1.5rem;
  border-radius: 2rem;
  cursor: pointer;
  transition: background 0.2s, color 0.2s;
}
.genre:hover {
  background: #e50914;
  color: #fff;
}
@media (max-width: 700px) {
  .genres-container h2 {
    font-size: 1.1rem;
  }
  .genres-section {
    padding: 1.2rem 0 1rem 0;
  }
  .genre {
    font-size: 0.9rem;
    padding: 0.5rem 1rem;
  }
}
</style>
