<template>
  <section id="about" class="about">
    <div class="container">
      <h2 data-aos="fade-up">Tentang Kami</h2>
      <div class="about-content">
        <div class="about-text" data-aos="fade-right">
          <p>Sederek Kopi adalah tempat di mana passion untuk kopi bertemu dengan keramahan. Kami memilih biji kopi terbaik dan meraciknya dengan penuh dedikasi untuk menghadirkan pengalaman kopi yang tak terlupakan.</p>
        </div>
        <div class="about-image" data-aos="fade-left">
          <img src="https://images.unsplash.com/photo-1442512595331-e89e73853f31?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" loading="lazy" alt="Coffee Brewing" />
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
// Component logic here if needed
</script>

<style scoped>
.about {
  padding: 80px 0;
  background: var(--background-color);
}

.about h2 {
  text-align: center;
  margin-bottom: 40px;
  color: var(--text-color);
}

.about-content {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 40px;
  align-items: center;
}

.about-text p {
  font-size: 1.1em;
  line-height: 1.8;
  color: var(--text-color);
}

.about-image img {
  width: 100%;
  border-radius: 10px;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
}

@media (max-width: 768px) {
  .about-content {
    grid-template-columns: 1fr;
  }

  .about-image {
    order: -1;
  }
}
</style>