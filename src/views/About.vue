<template>
  <div class="about">
    <header class="about-header">
      <h1>Our Story</h1>
      <p>Welcome to BlackEndpoints, your go-to platform for discovering and supporting Black-owned businesses in your
        community and beyond. We are on a mission to empower the Black community by bridging the gap between consumers
        and Black entrepreneurs through innovation and connectivity.</p>
<br/>
        <p>At BlackEndpoints, we believe that economic empowerment is the foundation of progress. Our platform provides an
        easy-to-use directory where users can find, explore, and support Black-owned businesses, whether you're looking
        for local gems or national brands.</p>
        <br/>
        <p>We're more than just a directory—we're building a movement. By connecting consumers with Black entrepreneurs, we
        aim to amplify Black voices, inspire community growth, and foster lasting change.</p>
        <br/>
        <p>Whether you’re a consumer passionate about buying Black or a business owner looking to expand your reach,
        BlackEndpoints is here to be your partner in progress.</p>
        <br/>
        <p>Join us as we create a future where access and opportunity thrive, one connection at a time. Together, we can
        build stronger communities and drive meaningful impact.</p>
        <br/>
        <p>Let’s redefine the way we connect. Let’s build together.</p>
    </header>

    <section class="team">
      <h2>Meet Our Team</h2>
      <div class="team-members">
        <div class="team-member">
          <img src="https://via.placeholder.com/150" alt="Jay">
          <h3>Jay</h3>
          <p class="role">Founder & CEO</p>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. In bibendum massa nec magna sodales congue.
            Integer rhoncus odio id erat mattis commodo. Nulla condimentum nisi a sem rutrum, sed lacinia ante lobortis.
            Pellentesque tortor nisl, fermentum varius quam ut, mattis aliquet mi. In hac habitasse platea dictumst.
            Suspendisse eleifend facilisis eleifend. Nulla viverra tempor dui ut porttitor.</p>
        </div>

        <div class="team-member">
          <img src="https://via.placeholder.com/150" alt="Michael Chen">
          <h3>Bri</h3>
          <p class="role">Founder & CTO</p>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. In bibendum massa nec magna sodales congue.
            Integer rhoncus odio id erat mattis commodo. Nulla condimentum nisi a sem rutrum, sed lacinia ante lobortis.
            Pellentesque tortor nisl, fermentum varius quam ut, mattis aliquet mi. In hac habitasse platea dictumst.
            Suspendisse eleifend facilisis eleifend. Nulla viverra tempor dui ut porttitor.</p>
        </div>

        <div class="team-member">
          <img src="https://via.placeholder.com/150" alt="Michael Chen">
          <h3>Alex</h3>
          <p class="role">Head of Product</p>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. In bibendum massa nec magna sodales congue.
            Integer rhoncus odio id erat mattis commodo. Nulla condimentum nisi a sem rutrum, sed lacinia ante lobortis.
            Pellentesque tortor nisl, fermentum varius quam ut, mattis aliquet mi. In hac habitasse platea dictumst.
            Suspendisse eleifend facilisis eleifend. Nulla viverra tempor dui ut porttitor.</p>
        </div>


        <div class="team-member">
          <img src="https://via.placeholder.com/150" alt="Michael Chen">
          <h3>Pat</h3>
          <p class="role">Head of Product</p>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. In bibendum massa nec magna sodales congue.
            Integer rhoncus odio id erat mattis commodo. Nulla condimentum nisi a sem rutrum, sed lacinia ante lobortis.
            Pellentesque tortor nisl, fermentum varius quam ut, mattis aliquet mi. In hac habitasse platea dictumst.
            Suspendisse eleifend facilisis eleifend. Nulla viverra tempor dui ut porttitor.</p>
        </div>


        <div class="team-member">
          <img src="https://via.placeholder.com/150" alt="Michael Chen">
          <h3>Wally</h3>
          <p class="role">Head of Product</p>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. In bibendum massa nec magna sodales congue.
            Integer rhoncus odio id erat mattis commodo. Nulla condimentum nisi a sem rutrum, sed lacinia ante lobortis.
            Pellentesque tortor nisl, fermentum varius quam ut, mattis aliquet mi. In hac habitasse platea dictumst.
            Suspendisse eleifend facilisis eleifend. Nulla viverra tempor dui ut porttitor.</p>
        </div>

      </div>
    </section>
  </div>
</template>

<style scoped>
.about {
  max-width: 1200px;
  margin: 0 auto;
  padding: 2rem;
}

.about-header {
  text-align: center;
  padding: 4rem 0;
  color: var(--text-color);
}

.about-header h1 {
  font-size: 3rem;
  margin-bottom: 1rem;
}

.team {
  margin: 4rem 0;
}

.team h2 {
  text-align: center;
  margin-bottom: 3rem;
  color: var(--text-color);
}

.team-members {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
}

.team-member {
  text-align: center;
  padding: 2rem;
  background-color: var(--card-bg);
  border-radius: 8px;
  transition: transform 0.3s;
  color: var(--text-color);
}

.team-member:hover {
  transform: translateY(-5px);
}

.team-member img {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  margin-bottom: 1rem;
}

.team-member h3 {
  margin: 1rem 0 0.5rem;
}

.role {
  color: var(--text-color);
  opacity: 0.7;
  font-style: italic;
  margin-bottom: 1rem;
}

@media (max-width: 768px) {
  .about {
    padding: 1rem;
  }

  .about-header {
    padding: 2rem 0;
  }

  .about-header h1 {
    font-size: 2.5rem;
  }

  .team {
    margin: 2rem 0;
  }

  .team-members {
    grid-template-columns: 1fr;
    gap: 1.5rem;
  }

  .team-member {
    padding: 1.5rem;
  }
}

@media (min-width: 769px) and (max-width: 1024px) {
  .about {
    padding: 1.5rem;
  }

  .team-members {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (min-width: 1440px) {
  .about {
    max-width: 1400px;
  }

  .team-members {
    gap: 3rem;
  }
}
</style>