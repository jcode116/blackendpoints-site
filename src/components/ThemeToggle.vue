<template>
  <button @click="themeStore.toggleTheme()" class="theme-toggle" :title="themeStore.isDark ? 'Switch to Light Mode' : 'Switch to Dark Mode'">
    <span v-if="themeStore.isDark">🌞</span>
    <span v-else>🌙</span>
  </button>
</template>

<script>
import { useThemeStore } from '../stores/theme'

export default {
  setup() {
    const themeStore = useThemeStore()
    return { themeStore }
  }
}
</script>

<style scoped>
.theme-toggle {
  background: none;
  border: none;
  cursor: pointer;
  font-size: 1.5rem;
  padding: 0.5rem;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: transform 0.3s ease;
}

.theme-toggle:hover {
  transform: scale(1.1);
}

@media (max-width: 768px) {
  .theme-toggle {
    margin-top: 0.5rem;
  }
}
</style>