<template>
  <div class="app">
    <!-- Header/Navbar -->
    <header :class="{ 'scrolled': isScrolled }" ref="header">
      <nav class="container">
        <div class="logo">
          <img src="./assets/logo.svg" alt="Sederek Kopi Logo" />
        </div>
       
      </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
      <swiper
        class="hero-slider"
        :modules="[SwiperAutoplay, SwiperEffectFade]"
        :autoplay="{ delay: 5000, disableOnInteraction: false }"
        :effect="'fade'"
        :loop="true"
      >
        <swiper-slide>
          <div class="hero-slide" style="background-image: url('https://images.unsplash.com/photo-1495474472287-4d71bcdd2085?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80')">
            <div class="container hero-content">
              <div class="hero-text">
                <h1 data-aos="fade-up">Selamat Datang di <span class="highlight">Sederek Kopi</span></h1>
                <p data-aos="fade-up" data-aos-delay="200">Nikmati secangkir kopi berkualitas dalam suasana yang nyaman</p>
                <div class="hero-buttons" data-aos="fade-up" data-aos-delay="400">
                  <a href="#menu" class="cta-button primary">Lihat Menu <i class="fas fa-arrow-right"></i></a>
                  <a href="#about" class="cta-button secondary">Tentang Kami <i class="fas fa-info-circle"></i></a>
                </div>
              </div>
              <div class="hero-features" data-aos="fade-left" data-aos-delay="600">
                <div class="feature-item">
                  <i class="fas fa-coffee"></i>
                  <h3>Kopi Berkualitas</h3>
                  <p>Biji kopi pilihan terbaik</p>
                </div>
                <div class="feature-item">
                  <i class="fas fa-clock"></i>
                  <h3>Buka Setiap Hari</h3>
                  <p>16.00 - 00.00 WIB</p>
                </div>
                <div class="feature-item">
                  <i class="fas fa-wifi"></i>
                  <h3>Free Wi-Fi</h3>
                  <p>Internet cepat & stabil</p>
                </div>
              </div>
            </div>
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="hero-slide" style="background-image: url('https://images.unsplash.com/photo-1442512595331-e89e73853f31?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80')">
            <div class="container hero-content">
              <div class="hero-text">
                <h1 data-aos="fade-up">Kopi Pilihan <span class="highlight">Terbaik</span></h1>
                <p data-aos="fade-up" data-aos-delay="200">Diracik dengan penuh dedikasi untuk pengalaman kopi terbaik</p>
                <div class="hero-buttons" data-aos="fade-up" data-aos-delay="400">
                  <a href="#menu" class="cta-button primary">Lihat Menu <i class="fas fa-arrow-right"></i></a>
                  <a href="#about" class="cta-button secondary">Tentang Kami <i class="fas fa-info-circle"></i></a>
                </div>
              </div>
              <div class="hero-features" data-aos="fade-left" data-aos-delay="600">
                <div class="feature-item">
                  <i class="fas fa-leaf"></i>
                  <h3>100% Organik</h3>
                  <p>Biji kopi organik</p>
                </div>
                <div class="feature-item">
                  <i class="fas fa-award"></i>
                  <h3>Kualitas Terjamin</h3>
                  <p>Standar mutu tinggi</p>
                </div>
                <div class="feature-item">
                  <i class="fas fa-hand-holding-heart"></i>
                  <h3>Pelayanan Terbaik</h3>
                  <p>Barista profesional</p>
                </div>
              </div>
            </div>
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="hero-slide" style="background-image: url('https://images.unsplash.com/photo-1501339847302-ac426a4a7cbb?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80')">
            <div class="container hero-content">
              <div class="hero-text">
                <h1 data-aos="fade-up">Suasana yang <span class="highlight">Nyaman</span></h1>
                <p data-aos="fade-up" data-aos-delay="200">Tempat ideal untuk bersantai dan menikmati kopi</p>
                <div class="hero-buttons" data-aos="fade-up" data-aos-delay="400">
                  <a href="#menu" class="cta-button primary">Lihat Menu <i class="fas fa-arrow-right"></i></a>
                  <a href="#about" class="cta-button secondary">Tentang Kami <i class="fas fa-info-circle"></i></a>
                </div>
              </div>
              <div class="hero-features" data-aos="fade-left" data-aos-delay="600">
                <div class="feature-item">
                  <i class="fas fa-couch"></i>
                  <h3>Tempat Nyaman</h3>
                  <p>Interior modern</p>
                </div>
                <div class="feature-item">
                  <i class="fas fa-music"></i>
                  <h3>Musik Akustik</h3>
                  <p>Suasana santai</p>
                </div>
                <div class="feature-item">
                  <i class="fas fa-parking"></i>
                  <h3>Area Parkir</h3>
                  <p>Parkir luas & aman</p>
                </div>
              </div>
            </div>
          </div>
        </swiper-slide>
      </swiper>
    </section>


    <!-- Menu Section -->
    <section id="menu" class="menu">
      <div class="container">
        <h2 class="special-menu-title" data-aos="fade-up">Menu Kami</h2>
        <div class="menu-grid">
          <div class="menu-item" data-aos="fade-up">
            <img src="https://images.unsplash.com/photo-1514432324607-a09d9b4aefdd?ixlib=rb-1.2.1&auto=format&fit=crop&w=634&q=80" loading="lazy" alt="Espresso" />
            <h3>Espresso</h3>
            <p>Rp 18.000</p>
          </div>
          <div class="menu-item" data-aos="fade-up" data-aos-delay="100">
            <img src="https://images.unsplash.com/photo-1534687941688-13aed7b21ff8?ixlib=rb-1.2.1&auto=format&fit=crop&w=634&q=80" loading="lazy" alt="Cappuccino" />
            <h3>Cappuccino</h3>
            <p>Rp 25.000</p>
          </div>
          <div class="menu-item" data-aos="fade-up" data-aos-delay="200">
            <img src="https://images.unsplash.com/photo-1517701604599-bb29b565090c?ixlib=rb-1.2.1&auto=format&fit=crop&w=634&q=80"  loading="lazy" alt="Latte" />
            <h3>Café Latte</h3>
            <p>Rp 23.000</p>
          </div>
          <div class="menu-item" data-aos="fade-up" data-aos-delay="300">
            <img src="https://images.unsplash.com/photo-1594631252845-29fc4cc8cde9?ixlib=rb-1.2.1&auto=format&fit=crop&w=634&q=80" loading="lazy" alt="V60" />
            <h3>V60</h3>
            <p>Rp 20.000</p>
          </div>
        </div>

        <h3 class="special-menu-title" data-aos="fade-up">Menu Spesial</h3>
        <div class="special-menu-container">
          <div class="special-menu-slider">
            <swiper
              :modules="[Autoplay, Pagination]"
              :slides-per-view="3"
              :space-between="30"
              :autoplay="{ delay: 3000, disableOnInteraction: false }"
              :pagination="{
                el: '.swiper-pagination',
                clickable: true,
                bulletClass: 'swiper-pagination-bullet radio-bullet'
              }"
              :breakpoints="{
                '320': { slidesPerView: 1, spaceBetween: 20 },
                '640': { slidesPerView: 2, spaceBetween: 20 },
                '768': { slidesPerView: 3, spaceBetween: 30 }
              }"
            >
            <swiper-slide>
              <div class="menu-item">
                <img src="https://images.unsplash.com/photo-1461023058943-07fcbe16d735?ixlib=rb-1.2.1&auto=format&fit=crop&w=634&q=80" loading="lazy" alt="Affogato" />
                <h3>Affogato</h3>
                <p>Rp 28.000</p>
              </div>
            </swiper-slide>
            <swiper-slide>
              <div class="menu-item">
                <img src="https://images.unsplash.com/photo-1572442388796-11668a67e53d?ixlib=rb-1.2.1&auto=format&fit=crop&w=634&q=80" loading="lazy" alt="Mocha" />
                <h3>Mocha</h3>
                <p>Rp 27.000</p>
              </div>
            </swiper-slide>
            <swiper-slide>
              <div class="menu-item">
                <img src="https://images.unsplash.com/photo-1579888944880-d98341245702?ixlib=rb-1.2.1&auto=format&fit=crop&w=634&q=80" loading="lazy" alt="Cold Brew" />
                <h3>Cold Brew</h3>
                <p>Rp 25.000</p>
              </div>
            </swiper-slide>
            <swiper-slide>
              <div class="menu-item">
                <img src="https://images.unsplash.com/photo-1461023058943-07fcbe16d735?ixlib=rb-1.2.1&auto=format&fit=crop&w=634&q=80" loading="lazy" alt="Caramel Macchiato" />
                <h3>Caramel Macchiato</h3>
                <p>Rp 30.000</p>
              </div>
            </swiper-slide>
            </swiper>
            <div class="swiper-pagination"></div>
          </div>
        </div>
      </div>
    </section>

    <!-- About Section -->
    <AboutUs />

    <!-- Location Section -->
    <Location />

    <!-- Footer -->
    <footer>
      <div class="container">
        <div class="footer-content">
          <div class="footer-logo">
            <img src="./assets/logo.svg" alt="Sederek Kopi Logo" />
          </div>
          <div class="social-links">
            <a href="#" target="_blank"><i class="fab fa-instagram"></i></a>
            <a href="#" target="_blank"><i class="fab fa-facebook"></i></a>
            <a href="#" target="_blank"><i class="fab fa-twitter"></i></a>
          </div>
        </div>
        <div class="footer-bottom">
          <p>&copy; 2024 Sederek Kopi. All rights reserved.</p>
        </div>
      </div>
    </footer>
  </div>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from 'vue'
import { Swiper, SwiperSlide } from 'swiper/vue'
import { Autoplay, EffectFade, Pagination } from 'swiper/modules'
import 'swiper/css/pagination'
import 'swiper/css'
import 'swiper/css/effect-fade'
import 'aos/dist/aos.css'
import '@fortawesome/fontawesome-free/css/all.css'
import AOS from 'aos'

// Import components
import AboutUs from './components/AboutUs.vue'
import Location from './components/Location.vue'

const isScrolled = ref(false)
const isMenuOpen = ref(false)
const header = ref(null)

const swiperModules = [Autoplay, EffectFade, Navigation]
const SwiperAutoplay = Autoplay
const SwiperEffectFade = EffectFade

const handleScroll = () => {
  if (window.scrollY > 50) {
    isScrolled.value = true
  } else {
    isScrolled.value = false
  }
}

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value
}

const closeMenu = () => {
  isMenuOpen.value = false
}

onMounted(() => {
  AOS.init({
    duration: 1000,
    easing: 'ease-in-out',
    once: true
  })

  window.addEventListener('scroll', handleScroll)
})

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll)
})
</script>

<style>
:root {
  --primary-color: #4CAF50;
  --secondary-color: #2E7D32;
  --text-color: #333;
  --light-text: #fff;
  --background-color: #f5f5f5;
  --header-height: 80px;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  font-family: 'Arial', sans-serif;
  line-height: 1.6;
  color: var(--text-color);
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

/* Header Styles */
header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background: rgba(0, 0, 0, 0.2);
  backdrop-filter: blur(10px);
  z-index: 1000;
  transition: all 0.3s ease;
  border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

header.scrolled {
  background: rgba(76, 175, 80, 0.95);
  backdrop-filter: blur(10px);
  box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
}

nav {
  height: var(--header-height);
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  position: relative;
  padding: 10px;
  transition: transform 0.3s ease;
}

.logo:hover {
  transform: scale(1.05);
}

.logo::before {
  content: '';
  position: absolute;
  top: -2px;
  left: -2px;
  right: -2px;
  bottom: -2px;
  background: linear-gradient(45deg, var(--primary-color), var(--secondary-color));
  border-radius: 10px;
  z-index: -1;
  opacity: 0;
  transition: opacity 0.3s ease;
}

.logo:hover::before {
  opacity: 1;
}

.logo img {
  height: 60px;
  filter: drop-shadow(0 2px 4px rgba(0, 0, 0, 0.2));
}

.nav-link {
  color: var(--light-text);
  text-decoration: none;
  margin-left: 30px;
  font-weight: 500;
  transition: all 0.3s ease;
  display: flex;
  align-items: center;
  padding: 8px 16px;
  border-radius: 20px;
}

.nav-link i {
  margin-right: 8px;
  font-size: 1.1em;
}

.nav-link:hover {
  background: var(--secondary-color);
  transform: translateY(-2px);
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}

.menu-toggle {
  color: var(--light-text);
  font-size: 24px;
  cursor: pointer;
  width: 40px;
  height: 40px;
  border-radius: 50%;
  background: rgba(255, 255, 255, 0.1);
  backdrop-filter: blur(10px);
  display: flex;
  align-items: center;
  justify-content: center;
  transition: all 0.3s ease;
}

.menu-toggle:hover {
  background: rgba(255, 255, 255, 0.2);
  transform: scale(1.1);
}

.menu-toggle i {
  transition: transform 0.3s ease;
}

.menu-toggle:hover i {
  transform: rotate(90deg);
}

/* Hero Section */
.hero {
  height: 100vh;
  position: relative;
  color: var(--light-text);
}

.hero-slider {
  height: 100%;
}

.hero-slide {
  height: 100vh;
  background-size: cover;
  background-position: center;
  position: relative;
}

.hero-slide::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.4));
}

.hero-content {
  height: 100%;
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 50px;
  align-items: center;
  position: relative;
  z-index: 1;
}

.hero-text {
  text-align: left;
}

.hero h1 {
  font-size: 3.5rem;
  margin-bottom: 20px;
  line-height: 1.2;
}

.highlight {
  color: var(--primary-color);
  position: relative;
  display: inline-block;
}

.highlight::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 4px;
  background: var(--primary-color);
  transform: scaleX(0);
  transform-origin: right;
  transition: transform 0.3s ease;
}

.highlight:hover::after {
  transform: scaleX(1);
  transform-origin: left;
}

.hero p {
  font-size: 1.2rem;
  margin-bottom: 30px;
  opacity: 0.9;
}

.hero-buttons {
  display: flex;
  gap: 20px;
}

.cta-button {
  display: inline-flex;
  align-items: center;
  padding: 15px 30px;
  text-decoration: none;
  border-radius: 30px;
  font-weight: 600;
  transition: all 0.3s ease;
}

.cta-button i {
  margin-left: 10px;
  transition: transform 0.3s ease;
}

.cta-button:hover i {
  transform: translateX(5px);
}

.cta-button.primary {
  background: var(--primary-color);
  color: var(--light-text);
}

.cta-button.primary:hover {
  background: var(--secondary-color);
  transform: translateY(-2px);
  box-shadow: 0 4px 15px rgba(76, 175, 80, 0.4);
}

.cta-button.secondary {
  background: transparent;
  color: var(--light-text);
  border: 2px solid var(--light-text);
}

.cta-button.secondary:hover {
  background: var(--light-text);
  color: var(--primary-color);
  transform: translateY(-2px);
  box-shadow: 0 4px 15px rgba(255, 255, 255, 0.4);
}

.hero-features {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 30px;
}

.feature-item {
  background: rgba(255, 255, 255, 0.1);
  backdrop-filter: blur(10px);
  padding: 30px;
  border-radius: 20px;
  text-align: center;
  transition: all 0.3s ease;
}

.feature-item:hover {
  transform: translateY(-5px);
  background: rgba(255, 255, 255, 0.15);
}

.feature-item i {
  font-size: 2.5rem;
  color: var(--primary-color);
  margin-bottom: 15px;
}

.feature-item h3 {
  font-size: 1.2rem;
  margin-bottom: 10px;
}

.feature-item p {
  font-size: 0.9rem;
  opacity: 0.8;
  margin: 0;
}

/* About Section */
.about {
  padding: 100px 0;
  background: var(--background-color);
}

.about-content {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 50px;
  align-items: center;
}

.about-image img {
  width: 100%;
  border-radius: 10px;
}


/* Menu Section */
 .menu {
   padding: 100px 0;
 }

 .menu-grid {
   display: grid;
   grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
   gap: 30px;
   margin-top: 50px;
   margin-bottom: 50px;
 }

 .menu-item {
   text-align: center;
   background: #fff;
   border-radius: 10px;
   overflow: hidden;
   box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
   transition: transform 0.3s ease;
 }

 .menu-item:hover {
   transform: translateY(-5px);
 }

 .menu-item img {
   width: 100%;
   height: 200px;
   object-fit: cover;
 }

 .menu-item h3 {
   margin: 15px 0 10px;
 }

 .special-menu-title {
   text-align: center;
   margin-bottom: 30px;
   color: var(--primary-color);
 }

 .special-menu-container {
  position: relative;
  margin-top: 2rem;
  padding: 0 40px;
}

.special-menu-slider {
  width: 100%;
}

.special-menu-slider .menu-item {
  height: 100%;
  margin: 10px;
}

.swiper-slide {
  height: auto;
}

.swiper-pagination {
  position: static;
  margin-top: 20px;
}

.radio-bullet {
  width: 16px !important;
  height: 16px !important;
  background-color: #ddd !important;
  border: 2px solid var(--primary-color) !important;
  opacity: 1 !important;
  margin: 0 6px !important;
}

.radio-bullet.swiper-pagination-bullet-active {
  background-color: var(--primary-color) !important;
}

.radio-bullet:hover {
  background-color: var(--primary-color) !important;
  opacity: 0.8 !important;
}

/* Location Section */
.location {
  padding: 100px 0;
  background: var(--background-color);
}

.location-content {
  display: grid;
  grid-template-columns: 2fr 1fr;
  gap: 50px;
  margin-top: 50px;
}

.address {
  padding: 30px;
  background: #fff;
  border-radius: 10px;
  box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
}

.address h3 {
  margin-bottom: 20px;
}

.address p {
  margin-bottom: 15px;
}

.address i {
  color: var(--primary-color);
  margin-right: 10px;
}

/* Footer */
footer {
  background: var(--primary-color);
  color: var(--light-text);
  padding: 50px 0 20px;
}

.footer-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 30px;
}

.footer-logo img {
  height: 60px;
}

.social-links a {
  color: var(--light-text);
  font-size: 24px;
  margin-left: 20px;
  transition: color 0.3s ease;
}

.social-links a:hover {
  color: var(--secondary-color);
}

.footer-bottom {
  text-align: center;
  padding-top: 20px;
  border-top: 1px solid rgba(255, 255, 255, 0.1);
}

/* Responsive Design */
@media (max-width: 1024px) {
  .hero-content {
    grid-template-columns: 1fr;
    gap: 30px;
    padding: 50px 0;
  }

  .hero-text {
    text-align: center;
  }

  .hero-buttons {
    justify-content: center;
  }

  .hero-features {
    grid-template-columns: repeat(3, 1fr);
  }
}

@media (max-width: 768px) {
  .menu-toggle {
    display: flex;
  }

  .nav-links {
    position: fixed;
    top: var(--header-height);
    left: 0;
    width: 100%;
    height: calc(100vh - var(--header-height));
    background: rgba(0, 0, 0, 0.95);
    backdrop-filter: blur(10px);
    padding: 40px 20px;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    transform: translateX(100%);
    transition: all 0.5s cubic-bezier(0.77, 0, 0.175, 1);
  }

  .nav-links.active {
    transform: translateX(0);
  }

  .nav-link {
    margin: 15px 0;
    width: 80%;
    max-width: 300px;
    justify-content: flex-start;
    font-size: 1.2rem;
    opacity: 0;
    transform: translateX(50px);
    transition: all 0.3s ease;
  }

  .nav-links.active .nav-link {
    opacity: 1;
    transform: translateX(0);
  }

  .nav-links.active .nav-link:nth-child(1) { transition-delay: 0.1s; }
  .nav-links.active .nav-link:nth-child(2) { transition-delay: 0.2s; }
  .nav-links.active .nav-link:nth-child(3) { transition-delay: 0.3s; }
  .nav-links.active .nav-link:nth-child(4) { transition-delay: 0.4s; }

  .hero h1 {
    font-size: 2.5rem;
  }

  .hero-features {
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  }

  .hero-buttons {
    flex-direction: column;
    gap: 15px;
  }

  .cta-button {
    width: 100%;
    justify-content: center;
  }

  .about-content,
  .location-content {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 480px) {
  .hero h1 {
    font-size: 2rem;
  }

  .hero p {
    font-size: 1rem;
  }

  .feature-item {
    padding: 20px;
  }

  .feature-item i {
    font-size: 2rem;
  }

  .feature-item h3 {
    font-size: 1rem;
  }

  .feature-item p {
    font-size: 0.8rem;
  }
}
</style>
