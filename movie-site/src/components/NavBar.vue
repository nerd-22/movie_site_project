


<template>
  <nav class="navbar">
    <div class="navbar-brand">
      <img src="https://upload.wikimedia.org/wikipedia/commons/0/08/Netflix_2015_logo.svg" alt="Prime Box Logo" class="navbar-logo" />
      <span class="navbar-title-red">Prime</span>
      <span class="navbar-title">Box</span>
    </div>
    <ul class="navbar-links">
      <li><a href="#">Home</a></li>
      <li><a href="#">TV Shows</a></li>
      <li><a href="#">Movies</a></li>
      <li><a href="#">My List</a></li>
    </ul>
    <div class="navbar-actions">
      <button class="navbar-signin" @click="$emit('show-login')">Login</button>
      <button class="navbar-signup" @click="$emit('show-signup')">Sign Up</button>
      <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="User Avatar" class="navbar-avatar" />
    </div>
  </nav>
</template>

<style scoped>
.navbar {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 30;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0.75rem 3vw;
  background: rgba(20, 20, 20, 0.95);
  border-bottom: 1.5px solid #232323;
  box-shadow: 0 2px 8px 0 rgba(0,0,0,0.7);
  backdrop-filter: blur(8px);
}
.navbar-brand {
  display: flex;
  align-items: center;
  gap: 0.7rem;
  user-select: none;
}
.navbar-logo {
  height: 2.2rem;
  width: auto;
  filter: drop-shadow(0 2px 4px #000a);
}
.navbar-title-red {
  font-size: 2rem;
  font-weight: 900;
  color: #e50914;
  letter-spacing: -1px;
  margin-left: 0.2rem;
}
.navbar-title {
  font-size: 2rem;
  font-weight: 900;
  color: #fff;
  letter-spacing: -1px;
}
.navbar-links {
  display: flex;
  gap: 2.2rem;
  list-style: none;
  margin: 0;
  padding: 0;
}
.navbar-links li a {
  color: #fff;
  font-size: 1.1rem;
  font-weight: 500;
  text-decoration: none;
  transition: color 0.2s;
}
.navbar-links li a:hover,
.navbar-links li a:focus {
  color: #e50914;
}
.navbar-actions {
  display: flex;
  align-items: center;
  gap: 1.2rem;
}
.navbar-signin {
  background: #e50914;
  color: #fff;
  font-weight: 700;
  font-size: 1rem;
  padding: 0.6rem 1.5rem;
  border: none;
  border-radius: 0.3rem;
  box-shadow: 0 2px 8px 0 rgba(0,0,0,0.2);
  cursor: pointer;
  transition: background 0.2s, box-shadow 0.2s;
}
.navbar-signin:hover,
.navbar-signin:focus {
  background: #b0060f;
  box-shadow: 0 4px 16px 0 rgba(229,9,20,0.2);
}
.navbar-avatar {
  width: 2.2rem;
  height: 2.2rem;
  border-radius: 50%;
  border: 2px solid #fff2;
  object-fit: cover;
  cursor: pointer;
  transition: border 0.2s;
}
.navbar-avatar:hover,
.navbar-avatar:focus {
  border: 2px solid #e50914;
}
@media (max-width: 900px) {
  .navbar-links {
    gap: 1.2rem;
  }
  .navbar-title-red, .navbar-title {
    font-size: 1.3rem;
  }
  .navbar-logo {
    height: 1.3rem;
  }
}
@media (max-width: 700px) {
  .navbar-links {
    display: none;
  }
  .navbar {
    padding: 0.75rem 1vw;
  }
}
</style>

<script setup>
// No logic needed for static nav
</script>
