<template>
  <footer class="footer-section">
    <div class="footer-container">
      <div class="footer-links">
        <a href="#">FAQ</a>
        <a href="#">Help Center</a>
        <a href="#">Terms of Use</a>
        <a href="#">Privacy</a>
        <a href="#">Cookie Preferences</a>
        <a href="#">Corporate Information</a>
      </div>
      <div class="footer-brand">&copy; 2025 Prime Box. Inspired by Netflix.</div>
    </div>
  </footer>
</template>

<script setup>
// Static footer
</script>

<style scoped>
.footer-section {
  background: #181818;
  padding: 2.5rem 0 1.5rem 0;
  border-top: 1.5px solid #232323;
}
.footer-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 3vw;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.footer-links {
  display: flex;
  flex-wrap: wrap;
  gap: 1.5rem;
  justify-content: center;
  margin-bottom: 1.2rem;
}
.footer-links a {
  color: #b3b3b3;
  font-size: 1rem;
  text-decoration: none;
  transition: color 0.2s;
}
.footer-links a:hover {
  color: #e50914;
}
.footer-brand {
  color: #888;
  font-size: 0.95rem;
  text-align: center;
}
@media (max-width: 700px) {
  .footer-links {
    gap: 0.7rem;
    font-size: 0.9rem;
  }
  .footer-section {
    padding: 1.2rem 0 0.7rem 0;
  }
}
</style>
