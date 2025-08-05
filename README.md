# 🌿💧 FarmEase: Solusi Manajemen Pertanian Lahan Kering untuk Petani Kupang

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)  
**Laravel v12.x** | **Bootstrap v5.3** | **Font Awesome** | **Vite + TypeScript**

---

## 📖 Tentang Proyek

**FarmEase** adalah sistem informasi manajemen pertanian berbasis web, dirancang untuk membantu petani kecil penggarap lahan kering di **Kabupaten Kupang, Nusa Tenggara Timur**.

Menanggapi tantangan iklim, efisiensi biaya, dan akses informasi, FarmEase hadir sebagai solusi digital yang intuitif dan ringan digunakan, baik oleh petani maupun penyuluh.

> 🎯 *Proyek ini dikembangkan sebagai bagian dari [Sebutkan nama kompetisi atau tujuan lain]*

---

## ✨ Fitur Utama

### 🌱 Perencanaan Musim Tanam Adaptif
- Mencatat dan memantau jadwal tanam & panen.
- Rekomendasi tanaman cocok berdasarkan kondisi lahan dan pola iklim.

### 💰 Pencatatan Input & Biaya Pertanian
- Pencatatan pupuk, pestisida, benih, dan operasional.
- Analisis efisiensi pengeluaran.

### ☁️ Informasi Cuaca & Agroklimat Lokal *(Simulasi)*
- Data curah hujan & suhu untuk wilayah Kupang.
- *(Rencana integrasi API cuaca real-time di masa depan).*

### 📈 Harga Pasar Komoditas *(Simulasi)*
- Harga pasar terkini komoditas utama.
- *(Rencana integrasi API pasar lokal di masa depan).*

---

## 🚀 Teknologi yang Digunakan

### Backend
- PHP 8.x
- Laravel 12.x
- SQLite (default dev) / MySQL (opsional)

### Frontend
- Vite (bundler modern, dukung HMR)
- TypeScript (untuk struktur dan skalabilitas)
- HTML5, CSS3, JavaScript (vanilla)
- Bootstrap 5.3 (via CDN)
- Font Awesome 6 (via CDN)
- Google Fonts: Poppins
- Animate.css *(opsional)*

---

## ⚙️ Instalasi & Setup Proyek

### 1. Clone Repo
```bash
git clone https://github.com/Hendrasetiawanolybunga/FarmEase.git
cd FarmEase
````

### 2. Install Dependency Backend (Laravel)

```bash
composer install
```

### 3. Konfigurasi `.env` & Generate App Key

```bash
cp .env.example .env
php artisan key:generate
```

---

## 🗃️ Setup Database

### ⚡ SQLite (rekomendasi untuk dev cepat)

* Pastikan `.env` memiliki:

  ```env
  DB_CONNECTION=sqlite
  DB_DATABASE=database/database.sqlite
  ```
* Buat file kosong:

  ```bash
  touch database/database.sqlite
  php artisan migrate
  ```

### 🛢️ MySQL (opsional)

* Ubah `.env`:

  ```env
  DB_CONNECTION=mysql
  DB_HOST=127.0.0.1
  DB_PORT=3306
  DB_DATABASE=farmease_db
  DB_USERNAME=root
  DB_PASSWORD=your_password
  ```
* Buat DB via phpMyAdmin atau CLI, lalu jalankan:

  ```bash
  php artisan migrate
  ```

---

## 🖥️ Menjalankan Laravel + Vite

### 1. Install Dependency Frontend (Vite + TS)

```bash
npm install
```

### 2. Jalankan Vite Dev Server

```bash
npm run dev
```

### 3. Jalankan Laravel Server

```bash
php artisan serve
```

Buka [http://127.0.0.1:8000](http://127.0.0.1:8000) di browser.
Pastikan `npm run dev` tetap aktif selama development untuk melihat perubahan secara real-time (Hot Module Replacement).

---

## ⚒️ Build untuk Produksi

```bash
npm run build
```

---

## 📂 Struktur Proyek Ringkas

```
├── app/
├── database/
│   └── database.sqlite
├── public/
├── resources/
│   ├── js/         # Berisi file TypeScript/JavaScript
│   ├── sass/       # (Opsional) SCSS jika digunakan
│   └── views/      # Blade Templates
├── routes/
├── vite.config.ts  # Konfigurasi Vite
└── tsconfig.json   # Konfigurasi TypeScript

## 🛣️ Roadmap Pengembangan

* ✅ Setup dasar Laravel + SQLite + Vite
* 🔲 CRUD lengkap semua modul (tanaman, biaya, musim tanam, dll)
* 🔲 Otentikasi pengguna (admin/petani)
* 🔲 Integrasi API Cuaca (OpenWeatherMap atau serupa)
* 🔲 Integrasi API Harga Pasar
* 🔲 Fitur notifikasi jadwal panen/cuaca
* 🔲 Grafik & laporan produksi/biaya
* 🔲 Modul komunikasi untuk kelompok tani/penyuluh



## 🤝 Kontribusi

Kami terbuka untuk:

* Pull request (fitur baru, perbaikan bug, dokumentasi)
* Diskusi ide baru (buka issue!)
* Pengujian dan pelaporan bug

> 💡 *Gunakan branch dan pull request terpisah untuk kontribusi.*


## 📫 Kontak

**Hendra Setiawan**
📧 [setia170104@gmail.com](mailto:setia170104@gmail.com)
🔗 [LinkedIn](https://www.linkedin.com/in/hendra-setiawan17/)
🐙 GitHub: [BlueCode46](https://github.com/Hendrasetiawanolybunga)


## 📝 Lisensi

Proyek ini dilisensikan di bawah lisensi **MIT**.
Silakan gunakan, ubah, dan distribusikan dengan bebas selama mencantumkan atribusi.


> Dibuat dengan ❤️ untuk memberdayakan petani lahan kering di Kupang.


### Catatan Penting:
- Kalau belum punya `Node.js`, instal dulu dari https://nodejs.org (gunakan versi LTS).


