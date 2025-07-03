# Sederek Kopi Website

Website untuk kedai kopi Sederek Kopi yang dibangun menggunakan Vue.js dan Vite.

## Teknologi yang Digunakan

- Vue.js 3
- Vite
- Swiper
- AOS (Animate On Scroll)
- Font Awesome

## Cara Menjalankan Proyek

1. Install dependencies:
```bash
npm install
```

2. Jalankan server development:
```bash
npm run dev
```

3. Build untuk production:
```bash
npm run build
```

## Deployment ke Vercel

1. Push kode ke repository GitHub

2. Buat akun di [Vercel](https://vercel.com) jika belum memiliki

3. Di dashboard Vercel:
   - Klik "New Project"
   - Import repository dari GitHub
   - Pilih repository sederek-kopi
   - Klik "Deploy"

Vercel akan otomatis mendeteksi konfigurasi Vue.js dan melakukan build dan deployment.

## Struktur Proyek

```
sederek-kopi/
├── src/
│   ├── assets/        # Gambar, font, dll
│   ├── components/    # Komponen Vue
│   ├── App.vue        # Root component
│   └── main.js        # Entry point
├── public/            # Static files
├── index.html         # HTML template
├── vite.config.js     # Konfigurasi Vite
├── vercel.json        # Konfigurasi Vercel
└── package.json       # Dependencies dan scripts
```

## Fitur

- Desain responsif
- Animasi scroll
- Slider menu
- Integrasi peta
- Optimasi untuk deployment
