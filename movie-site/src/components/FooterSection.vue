<template>
  <footer class="footer-section">
    <div class="footer-container">

       <!--Back to Top Button -->
      <button class="back-to-top" @click="scrollToTop" title="Back to top">
        ↑
      </button>
      <div class="footer-links">
        <a href="#">FAQ</a>
        <a href="#">Help Center</a>
        <a href="#">Terms of Use</a>
        <a href="#">Privacy</a>
        <a href="#">Cookie Preferences</a>
        <a href="#">Corporate Information</a>
      </div>
      
      <!-- Separator Line -->
      <div class="footer-separator"></div>
      
      <div class="footer-brand">&copy; 2025 Prime Box. Inspired by Netflix.</div>
    </div>
  </footer>
</template>

<script setup>
// Static footer
const scrollToTop = () => {
  window.scrollTo({
    top: 0,
    behavior: 'smooth'
  });
};
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

/*  Separator Styles */
.footer-separator {
  width: 80%;
  height: 1px;
  background: linear-gradient(
    90deg,
    transparent 0%,
    #e50914 30%,
    #e50914 70%,
    transparent 100%
  );
  margin: 1rem 0 1.2rem 0;
  opacity: 0.4;
  position: relative;
}
/* Back to Top Button */
.back-to-top {
  background: #e50914;
  color: white;
  border: none;
  border-radius: 50%;
  width: 45px;
  height: 45px;
  font-size: 1.2rem;
  cursor: pointer;
  margin-bottom: 1.5rem;
  transition: all 0.2s ease;
}

.back-to-top:hover {
  background: #f40612;
  transform: translateY(-3px);
}

.back-to-top:active {
  transform: translateY(0);
}
</style>