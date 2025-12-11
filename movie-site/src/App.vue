
<script setup>
import NavBar from './components/NavBar.vue'
import HeroSection from './components/HeroSection.vue'
import FeaturedMovies from './components/FeaturedMovies.vue'
import TrendingNow from './components/TrendingNow.vue'
import TopPicks from './components/TopPicks.vue'
import Genres from './components/Genres.vue'
import FooterSection from './components/FooterSection.vue'
</script>

<template>
  <div class="bg-black min-h-screen">
    <NavBar />
    <main>
      <HeroSection />
      <FeaturedMovies />
      <TrendingNow />
      <TopPicks />
      <Genres />
      <FooterSection />
    </main>
  </div>
</template>


