
<template>
  <section class="hero-section">
    <div class="hero-overlay"></div>
    <div class="hero-content">
      <h1>Unlimited movies, TV shows, and more.</h1>
      <p>Watch anywhere. Cancel anytime. Dive into the world of entertainment with <span class="primebox">Prime Box</span>.</p>
      <form class="hero-form">
        <input type="email" placeholder="Email address" />
        <button type="submit">Get Started</button>
      </form>
    </div>
  </section>
</template>

<script setup>
// No logic needed for static hero
</script>

<style scoped>
.hero-section {
  position: relative;
  display: flex;
  align-items: flex-start;
  justify-content: flex-start;
  min-height: 90vh;
  width: 100%;
  background: url('https://images.unsplash.com/photo-1504384308090-c894fdcc538d?auto=format&fit=crop&w=1500&q=80') center center/cover no-repeat;
  overflow: hidden;
}
.hero-overlay {
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(180deg,rgba(0,0,0,0.92) 60%,rgba(0,0,0,0.1) 100%);
  z-index: 1;
}
.hero-content {
  position: relative;
  z-index: 2;
  margin-top: 7vw;
  margin-left: 6vw;
  max-width: 700px;
  color: #fff;
}
.hero-content h1 {
  font-size: 3.2rem;
  font-weight: 900;
  line-height: 1.1;
  margin-bottom: 2rem;
  text-shadow: 0 4px 32px #000a, 0 2px 8px #000a;
}
.hero-content p {
  font-size: 1.5rem;
  font-weight: 500;
  margin-bottom: 2.5rem;
  color: #e5e5e5;
}
.primebox {
  color: #e50914;
  font-weight: 700;
}
.hero-form {
  display: flex;
  flex-direction: row;
  gap: 1rem;
}
.hero-form input[type="email"] {
  padding: 1.1rem 1.5rem;
  border-radius: 0.3rem;
  border: none;
  font-size: 1.1rem;
  width: 260px;
  max-width: 60vw;
  outline: none;
  color: #222;
}
.hero-form button {
  background: #e50914;
  color: #fff;
  font-weight: 700;
  font-size: 1.1rem;
  padding: 1.1rem 2.5rem;
  border: none;
  border-radius: 0.3rem;
  box-shadow: 0 2px 8px 0 rgba(0,0,0,0.2);
  cursor: pointer;
  transition: background 0.2s, box-shadow 0.2s;
}
.hero-form button:hover,
.hero-form button:focus {
  background: #b0060f;
  box-shadow: 0 4px 16px 0 rgba(229,9,20,0.2);
}
@media (max-width: 900px) {
  .hero-content h1 {
    font-size: 2.1rem;
  }
  .hero-content p {
    font-size: 1.1rem;
  }
  .hero-form input[type="email"] {
    padding: 0.7rem 1rem;
    font-size: 1rem;
  }
  .hero-form button {
    padding: 0.7rem 1.2rem;
    font-size: 1rem;
  }
}
@media (max-width: 600px) {
  .hero-content {
    margin-left: 3vw;
    margin-top: 18vw;
    max-width: 95vw;
  }
  .hero-form {
    flex-direction: column;
    gap: 0.7rem;
  }
  .hero-form input[type="email"] {
    width: 100%;
    max-width: 100vw;
  }
}
</style>
