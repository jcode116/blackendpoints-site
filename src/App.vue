<template>
  <div class="app">
    <nav class="navbar">
      <BrandLogo />
      <div class="nav-controls">
        <div class="nav-links">
          <router-link to="/about" class="nav-link">About Us</router-link>
          <router-link to="/directory" class="nav-link">Directory</router-link>
        </div>
        <ThemeToggle />
      </div>
    </nav>
    <router-view></router-view>
  </div>
</template>

<script>
import ThemeToggle from './components/ThemeToggle.vue'
import BrandLogo from './components/BrandLogo.vue'

export default {
  components: {
    ThemeToggle,
    BrandLogo
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

:root {
  --bg-color: white;
  --text-color: #333;
  --nav-bg: black;
  --nav-text: white;
  --card-bg: #f8f8f8;
  --border-color: #ddd;
  --input-bg: white;
  --input-border: black;
}

.dark-mode {
  --bg-color: #121212;
  --text-color: #e0e0e0;
  --nav-bg: #000;
  --nav-text: #fff;
  --card-bg: #1e1e1e;
  --border-color: #333;
  --input-bg: #2d2d2d;
  --input-border: #444;
}

body {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
  line-height: 1.6;
  color: var(--text-color);
  background-color: var(--bg-color);
  transition: background-color 0.3s, color 0.3s;
}

.app {
  min-height: 100vh;
  background-color: var(--bg-color);
}

.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
  background-color: var(--nav-bg);
  color: var(--nav-text);
}

.nav-controls {
  display: flex;
  align-items: center;
  gap: 2rem;
}

.nav-links {
  display: flex;
  gap: 2rem;
}

.nav-link {
  color: var(--nav-text);
  text-decoration: none;
  transition: opacity 0.3s;
}

.nav-link:hover {
  opacity: 0.8;
}

@media (max-width: 768px) {
  .navbar {
    flex-direction: column;
    padding: 1rem;
    gap: 1rem;
    text-align: center;
  }

  .nav-controls {
    flex-direction: column;
    gap: 1rem;
  }

  .nav-links {
    gap: 1rem;
    flex-direction: column;
    width: 100%;
  }

  .nav-link {
    display: block;
    padding: 0.5rem;
  }
}
</style>