<template>
  <div class="container">
    <div class="about">
      <h1>About us</h1>
      <p>
        Welcome - this is your passport to a world of exploration and adventure! We are passionate travel enthusiasts who believe 
        in the transformative power of discovering new places, cultures, and experiences.
      </p>
      <h1>Our mission</h1>
      <p>
        Our mission is to inspire and guide fellow travelers on their journey to explore the beauty and diversity our planet has to 
        offer. Whether you're a seasoned globetrotter or a first-time adventurer, our blog is here to ignite your wanderlust and 
        provide valuable insights for your next escapade.
      </p>
    </div>
  </div>
</template>

<style>
.container {
  display: flex;
  place-items: center;
}

.about {
  display: flex;
  flex-direction: column;
  justify-content: center; 
  height: 100vh; 
}

@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
  }
}
</style>