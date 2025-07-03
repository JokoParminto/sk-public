<template>
  <section id="location" class="location">
    <div class="container">
      <h2 data-aos="fade-up">Lokasi</h2>
      <div class="location-content">
        <div class="map" data-aos="fade-right">
         <iframe
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3952.7127396671584!2d110.38690521476882!3d-7.947248594827576!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e7a5560b52110fd%3A0x402c37b9f7e73990!2sSederek%20Kopi!5e0!3m2!1sen!2sid!4v1627894592754!5m2!1sen!2sid"
            width="100%"
            height="450"
            style="border:0;"
            allowfullscreen=""
            loading="lazy">
          </iframe>
        </div>
        <div class="address" data-aos="fade-left">
          <h3>Sederek Kopi</h3>
          <p><i class="fas fa-map-marker-alt"></i> Bantul, Daerah Istimewa Yogyakarta</p>
          <p><i class="fas fa-clock"></i> Buka Setiap Hari: 16.00 - 00.00</p>
          <p><i class="fas fa-tag"></i> Rp 1.000 - Rp 25.000</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
// Component logic here if needed
</script>

<style scoped>
.location {
  padding: 80px 0;
  background: #fff;
}

.location h2 {
  text-align: center;
  margin-bottom: 40px;
  color: var(--text-color);
}

.location-content {
  display: grid;
  grid-template-columns: 2fr 1fr;
  gap: 40px;
  align-items: start;
}

.map iframe {
  border-radius: 10px;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
}

.address {
  padding: 20px;
  background: var(--background-color);
  border-radius: 10px;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
}

.address h3 {
  margin-bottom: 20px;
  color: var(--primary-color);
}

.address p {
  margin: 10px 0;
  display: flex;
  align-items: center;
  gap: 10px;
}

.address i {
  color: var(--primary-color);
  width: 20px;
}

@media (max-width: 768px) {
  .location-content {
    grid-template-columns: 1fr;
  }

  .map iframe {
    height: 300px;
  }
}
</style>