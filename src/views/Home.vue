<template>
  <div class="home">
    <header class="hero">
      <h1>BlackEndpoints</h1>
      <p class="subtitle">Empowering developers with robust API solutions</p>
    </header>
    
    <section class="intro">
      <h2>Why Choose Us?</h2>
      <p>At BlackEndpoints, we're dedicated to simplifying API development and management. Our platform provides developers with the tools they need to build, test, and deploy APIs efficiently.</p>
    </section>

    <section class="newsletter">
      <h2>Stay Updated</h2>
      <p>Subscribe to our newsletter for the latest updates and features.</p>
      <form @submit.prevent="handleSubmit" class="newsletter-form">
        <input 
          type="email" 
          v-model="email" 
          placeholder="Enter your email"
          required
        >
        <button type="submit">Subscribe</button>
      </form>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      email: ''
    }
  },
  methods: {
    handleSubmit() {
      alert('Thank you for subscribing!')
      this.email = ''
    }
  }
}
</script>

<style scoped>
.home {
  max-width: 1200px;
  margin: 0 auto;
  padding: 2rem;
}

.hero {
  text-align: center;
  padding: 4rem 0;
}

.hero h1 {
  font-size: 3.5rem;
  margin-bottom: 1rem;
  color: var(--text-color);
}

.subtitle {
  font-size: 1.5rem;
  color: var(--text-color);
  opacity: 0.8;
}

.intro {
  margin: 4rem 0;
  padding: 2rem;
  background-color: var(--card-bg);
  border-radius: 8px;
}

.intro h2 {
  margin-bottom: 1rem;
  color: var(--text-color);
}

.newsletter {
  text-align: center;
  padding: 4rem 0;
}

.newsletter h2,
.newsletter p {
  color: var(--text-color);
}

.newsletter-form {
  display: flex;
  max-width: 500px;
  margin: 2rem auto;
  gap: 1rem;
}

input[type="email"] {
  flex: 1;
  padding: 0.8rem;
  border: 2px solid var(--input-border);
  border-radius: 4px;
  font-size: 1rem;
  background-color: var(--input-bg);
  color: var(--text-color);
}

button {
  padding: 0.8rem 2rem;
  background-color: var(--nav-bg);
  color: var(--nav-text);
  border: none;
  border-radius: 4px;
  cursor: pointer;
  transition: opacity 0.3s;
}

button:hover {
  opacity: 0.9;
}

@media (max-width: 768px) {
  .home {
    padding: 1rem;
  }

  .hero {
    padding: 2rem 0;
  }

  .hero h1 {
    font-size: 2.5rem;
  }

  .subtitle {
    font-size: 1.2rem;
  }

  .newsletter-form {
    flex-direction: column;
    padding: 0 1rem;
  }

  button {
    width: 100%;
  }
}

@media (min-width: 769px) and (max-width: 1024px) {
  .home {
    padding: 1.5rem;
  }

  .hero h1 {
    font-size: 3rem;
  }
}

@media (min-width: 1440px) {
  .home {
    max-width: 1400px;
  }

  .hero h1 {
    font-size: 4rem;
  }
}
</style>