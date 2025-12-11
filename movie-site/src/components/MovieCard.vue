<template>
  <div class="bg-zinc-900 rounded-lg overflow-hidden shadow-xl min-w-[200px] max-w-[220px] hover:scale-110 hover:z-10 transition-transform duration-300 cursor-pointer border-2 border-zinc-800 hover:border-red-600 relative">
    <div class="h-64 bg-zinc-800 flex items-center justify-center relative">
      <img src="https://image.tmdb.org/t/p/w500/8YFL5QQVPy3AgrEQxNYVSgiPEbe.jpg" alt="Movie Poster" class="object-cover w-full h-full" />
      <span class="absolute bottom-2 left-2 bg-black/70 text-xs text-white px-2 py-1 rounded">HD</span>
    </div>
    <div class="p-4">
      <h3 class="text-lg font-bold text-white mb-1 truncate">Movie Title</h3>
      <p class="text-gray-400 text-xs">Action, Adventure</p>
    </div>
  </div>
</template>

<script setup>
// Placeholder for movie card
</script>
