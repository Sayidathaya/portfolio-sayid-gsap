# ✨ Sayid Rafi A'thaya — Portfolio ✨
[portfolio-sayid.vercel.app](https://portfolio-sayid.vercel.app/)
> 🖤 *Dark. Elegant. Animated. Satu file HTML yang gak main-main.*

---

## 🚀 Apa Ini?

Portfolio pribadi **Sayid Rafi A'thaya** — seorang developer, moderator, dan tech enthusiast yang passionate banget di dunia AI dan komunikasi digital. Dibuat sebagai **Single Page Application (SPA)** murni: satu `index.html`, nol framework, nol drama. 💅

---

## 🎬 Animasi yang Ada (GSAP-powered)

| 🎞️ Animasi | 💡 Inspirasi |
|---|---|
| 🔢 Preloader counter 0→100% + slide exit | Spylt Preloader |
| 🔤 Nama hero muncul huruf per huruf | SplitText `chars` stagger |
| 📐 Section title reveal dari tengah | `clipPath polygon` reveal |
| 🌈 Teks about nyala kata per kata saat scroll | Word color scrub + ScrollTrigger |
| 🌀 Hero section miring saat di-scroll | `rotate + scale + yPercent` scrub |
| ↔️ Dua baris kata besar gerak berlawanan | `xPercent` horizontal scrub |
| 🃏 Kartu sertifikat muncul dari bawah | `yPercent` stagger |
| 📜 Marquee berjalan otomatis | `xPercent` infinite repeat |

---

## 📁 Struktur Folder

```
sayid-rafi-portfolio/
│
├── 📄 index.html                  ← Satu-satunya file yang kamu butuhkan!
│
└── 📂 assets/
    ├── 🖼️  foto-profil.jpg
    └── 📂 certificates/
        ├── 🏅 cert_responsible_ai.jpg
        ├── 🏅 cert_ibm_code.jpg
        ├── 🏅 cert_webinar_artikel.jpg
        ├── 🏅 cert_webinar_branding.jpg
        └── 🏅 cert_itech.jpg
```

---

## ⚡ Cara Pakai

### 1️⃣ Extract ZIP
```bash
unzip sayid-rafi-portfolio-v2.zip
```

### 2️⃣ Buka di browser
```bash
# Langsung dobel klik index.html, atau:
cd sayid-rafi-portfolio-v2
# pakai Live Server di VS Code (recommended)
# atau python buat local server:
python -m http.server 5500
```

### 3️⃣ Profit 🎉
Buka `http://localhost:5500` di browser dan nikmatin animasinya!

> ⚠️ **Butuh koneksi internet** saat pertama buka — untuk load font Google & GSAP dari CDN.

---

## 🛠️ Tech Stack

```
🏗️  HTML5          → Struktur utama (SPA)
🎨  CSS3           → Dark luxury design system
⚡  GSAP 3.12.5    → Semua animasi
🔠  SplitText      → Char & word splitting
📌  ScrollTrigger  → Scroll-linked animations
🔤  Playfair Display → Font display (serif elegan)
🔡  DM Sans        → Font body (clean & modern)
💻  DM Mono        → Font monospace (labels)
🎯  Remix Icon     → Ikon UI
```

---

## 🏅 Sertifikat yang Ditampilkan

| # | 🏆 Sertifikat | 🏢 Penyelenggara |
|---|---|---|
| 1 | 🤖 Certificate of Responsible AI | Remote Skills Academy × Google.org × ADB × AVPN |
| 2 | 💻 Code & Optimization — IBM Wave 4 | IBM Bootcamp |
| 3 | 📝 Moderator Webinar Penulisan Artikel | PT Serasi Publisher |
| 4 | 🌟 Moderator Webinar Personal Branding | Webinar Series |
| 5 | 🎪 Sekretaris & Bendahara — I-TECH | I-TECH Technology Event |

---

## 🎨 Design System

```css
/* Color Palette */
--bg:    #07070c   /* Background utama — hitam legam 🖤 */
--s1:    #0f0f16   /* Surface level 1 */
--s2:    #17171f   /* Surface level 2 */
--g1:    #c9a84c   /* Gold primary ✨ */
--g2:    #f0cb6e   /* Gold lighter */
--w:     #edeae2   /* Off-white text */
--mute:  #6a6a7a   /* Muted text */
```

---

## 🐛 Bug Fix Log

### v2-fix — Preloader Stuck 0% 🔧

**Masalah:**
- `SplitText.min.js` gagal load dari CDN → `gsap.registerPlugin()` error → seluruh script mati → counter preloader gak jalan 😵

**Fix yang dilakukan:**
- ✅ Preloader dipindah ke `<head>` sebagai script **terpisah** — berjalan sebelum GSAP
- ✅ Exit animation pakai CSS `transition` murni, **bukan** GSAP
- ✅ GSAP CDN diganti ke `cdnjs` (lebih stabil) + `unpkg` untuk SplitText
- ✅ Semua `SplitText.create()` dibungkus fallback `if(typeof SplitText !== 'undefined')`

---

## 📝 Kustomisasi

### Ganti Info Kontak
Cari dan ganti di `index.html`:
```
sayid.rafi@example.com  → email kamu
github.com/sayidrafi    → github kamu
linkedin.com/in/sayidrafi → linkedin kamu
@sayidrafi              → instagram kamu
```

### Ganti Foto Profil
Replace file `assets/foto-profil.jpg` dengan foto kamu (rasio 3:4 terbaik).

### Tambah Sertifikat Baru
1. Tambah gambar ke `assets/certificates/`
2. Duplikat satu blok `.cert-card` di HTML
3. Tambah data di object `CERTS` di bagian script

---

## 🌐 Deploy ke Internet

| Platform | Cara |
|---|---|
| 🟣 GitHub Pages | Upload folder → Settings → Pages → Deploy from branch |
| 🔺 Vercel | Drag & drop folder ke vercel.com |
| 🟠 Netlify | Drag & drop folder ke netlify.com/drop |

> 💡 Semua platform di atas **gratis** dan bisa live dalam hitungan menit!

---

## 📄 Lisensi

```
MIT License — bebas dipakai, dimodif, dan dishare.
Tapi kalau jadi portfolio kamu, jangan lupa ganti namanya ya 😄
```

---

<div align="center">

**Dibuat dengan 🖤 + ☕ + GSAP**

*Sayid Rafi A'thaya — 2025*

⭐ *Kalau suka, kasih bintang!* ⭐

</div>

![Banner](https://capsule-render.vercel.app/api?type=waving&height=240&color=0:0f172a,50:0f766e,100:0d9488&text=Kampung%20Ketupat%20Web&fontColor=ffffff&fontSize=46&fontAlignY=40&desc=Website%20Wisata%20%C2%B7%20PHP%20MVC%20%C2%B7%20Admin%20Panel%20%C2%B7%20MySQL&descAlignY=62&descSize=18)

<div align="center">

[![PHP](https://img.shields.io/badge/PHP-8.2+-777BB4?style=for-the-badge&logo=php&logoColor=white)](https://www.php.net/)
[![MySQL](https://img.shields.io/badge/MySQL-8.0+-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](https://www.mysql.com/)
[![License](https://img.shields.io/badge/License-MIT-22c55e?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![Status](https://img.shields.io/badge/Status-Live-0d9488?style=for-the-badge&logo=vercel&logoColor=white)](https://kampung-ketupat.infinityfree.me/)
[![MVC](https://img.shields.io/badge/Arsitektur-MVC-f59e0b?style=for-the-badge)](https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93controller)

</div>

---

## 🔗 Tautan Proyek

> Semua resource utama proyek ini dapat diakses melalui tautan berikut:

| Resource | Tautan |
|---|---|
| 🌐 **Website (Live Hosting)** | [kampung-ketupat.infinityfree.me](https://kampung-ketupat.infinityfree.me/) |
| 📊 **Presentasi / Slide Deck** | [Lihat di Canva](https://canva.link/54cr2ep7p6ouwdr) |
| 📄 **Laporan Proyek** | [Google Drive – Laporan](https://drive.google.com/drive/folders/1NnE_3vCfHOyXmjiId5lK8Y-TGkFcHNcU?usp=sharing) |
| 🎤 **Rekaman Wawancara** | [Google Drive – Wawancara](https://drive.google.com/drive/folders/1nMXrLRJ-9rJV7JU9HYuCDG_3R1cVz6eg?usp=sharing) |
| 🗺️ **Flowchart (Draw.io)** | [Lihat Flowchart](https://drive.google.com/file/d/1xvJ7Z_Qhu0zfzCXTjoyFLHQ2VosqakOO/view?usp=drive_link) |

---

## 📑 Daftar Isi

- [🎯 Ringkasan Proyek](#-ringkasan-proyek)
- [✨ Fitur Utama](#-fitur-utama)
- [🛠️ Stack Teknologi](#️-stack-teknologi)
- [🗂️ Struktur Folder](#️-struktur-folder)
- [🏗️ Arsitektur Aplikasi](#️-arsitektur-aplikasi)
- [🗃️ Skema Database](#️-skema-database)
- [🧭 Halaman & Route Website](#-halaman--route-website)
- [🔐 Fitur Keamanan](#-fitur-keamanan)
- [⚙️ Konfigurasi Environment](#️-konfigurasi-environment)
- [🚀 Quick Start (Instalasi Lokal)](#-quick-start-instalasi-lokal)
- [🌐 Deployment ke Hosting](#-deployment-ke-hosting)
- [🧪 Testing & Smoke Test](#-testing--smoke-test)
- [📸 Screenshoot Aplikasi](#-screenshot-aplikasi)
- [👥 Tim Pengembang](#-tim-pengembang)

---

## 🎯 Ringkasan Proyek

**Kampung Ketupat Web** adalah website profil dan publikasi informasi wisata yang dibangun untuk Kampung Ketupat — sebuah destinasi wisata lokal dengan identitas budaya dan kuliner yang kuat. Website ini dirancang agar konten dapat dikelola secara mandiri oleh pengelola kampung tanpa kebutuhan keahlian teknis tinggi.

Website ini menyediakan dua lapisan utama:

- **Sisi Publik** — Halaman yang dapat diakses siapa saja untuk menjelajahi informasi wisata, galeri foto, event, UMKM lokal, serta mengisi form kritik dan saran.
- **Sisi Admin (Panel Manajemen)** — Dashboard terproteksi untuk mengelola seluruh konten website melalui antarmuka CRUD yang intuitif.

Fokus utama pengembangan:

- **Kemudahan pengelolaan konten** — Admin dapat menambah, mengubah, dan menghapus konten tanpa menyentuh kode.
- **Antarmuka bersih & ringan** — Tidak bergantung pada framework berat; native PHP yang cepat dan mudah di-deploy.
- **Keamanan dasar yang solid** — CSRF protection, login throttle, session hardening, dan security logging sudah terpasang sejak awal.
- **Portabilitas tinggi** — Dapat berjalan di shared hosting maupun VPS dengan minimal konfigurasi.

---

## ✨ Fitur Utama

### 🌍 Halaman Publik

#### 🏠 Beranda (Landing Page)
- Ringkasan informasi utama Kampung Ketupat.
- Menampilkan highlight galeri, event terbaru, dan UMKM unggulan.
- Hero section dengan visual menarik.

#### 🖼️ Galeri
- Menampilkan koleksi foto publik yang sudah dipublish oleh admin.
- Filter berdasarkan **kategori konten**: `wisata`, `kuliner`, `budaya`, `fasilitas`, `umum`.
- Tampilan grid responsif.
- Admin dapat toggle publish/unpublish per foto, atau publish semua sekaligus.

#### 📅 Event
- Daftar event dengan informasi lengkap: nama, deskripsi, lokasi, tanggal mulai & selesai, jam mulai & jam selesai.
- Indikator **status event**: `Akan Datang`, `Berlangsung`, `Selesai`.
- Dukungan **link informasi tambahan** (misalnya ke media sosial atau pendaftaran).

#### 🏪 UMKM
- Menampilkan profil UMKM lokal Kampung Ketupat.
- Informasi mencakup: nama usaha, pemilik, kategori, deskripsi, produk unggulan, kontak, dan alamat.
- Upload dan tampil gambar produk/usaha.
- Kategori UMKM: `kuliner`, `kerajinan`, `souvenir`, `jasa`, `lainnya`.

#### 💬 Kritik & Saran
- Form masukan pengunjung dengan jenis pesan: `kritik`, `saran`, `pertanyaan`, `apresiasi`.
- Data tersimpan ke database dan menunggu moderasi admin.
- Admin menentukan apakah pesan ditampilkan ke publik atau tetap internal.

#### 📍 Lokasi & Kontak
- Informasi lokasi dan cara menghubungi pengelola Kampung Ketupat.

---

### 🛡️ Panel Admin

#### 🔑 Autentikasi
- Halaman login terproteksi di `/admin/login`.
- **Login throttle**: maksimal 5 percobaan dalam 10 menit, pemblokiran selama 15 menit jika melebihi batas.
- Session regenerasi ID setiap login untuk mencegah session fixation.
- Logout via POST request (mencegah CSRF pada logout).

#### 📊 Dashboard
- Statistik ringkasan: jumlah galeri, event, UMKM, dan pesan kritik saran yang belum dibaca.
- Tampilan data terkini di satu layar.

#### 🖼️ Manajemen Galeri
- **Tambah** foto baru dengan judul, deskripsi, kategori, dan upload gambar.
- **Edit** data foto yang sudah ada.
- **Hapus** foto (via POST, bukan GET — mencegah penghapusan tidak disengaja).
- **Toggle Publish/Unpublish** per foto.
- **Publish Semua** sekaligus dengan satu klik.

#### 📅 Manajemen Event
- **Tambah** event baru dengan form lengkap (nama, deskripsi, lokasi, tanggal, jam, link info, upload foto).
- **Edit** dan **Hapus** event.
- Manajemen status otomatis berdasarkan tanggal.

#### 🏪 Manajemen UMKM
- **Tambah**, **Edit**, dan **Hapus** data UMKM.
- Upload foto per UMKM, tersimpan di `public/assets/uploads/umkm/`.

#### 💬 Moderasi Kritik & Saran
- Daftar pesan **pending** yang belum diproses.
- Aksi: **Terima** (ubah status ke `diterima`), **Tampilkan** (jadikan `publik`), **Sembunyikan**, **Kembalikan ke pending**.
- Halaman **Arsip** pesan yang sudah diproses.
- Semua aksi moderasi menggunakan POST request + CSRF token.

---

## 🛠️ Stack Teknologi

| Kategori | Teknologi |
|---|---|
| **Backend Language** | PHP 8.2+ |
| **Database** | MySQL 8.0+ (via MySQLi) |
| **Arsitektur** | MVC Sederhana (Native PHP, tanpa framework) |
| **Frontend** | HTML5, CSS3, JavaScript (ES6+) |
| **UI Icons** | Bootstrap Icons |
| **Alert/Dialog** | SweetAlert2 |
| **Web Server** | Apache (dengan `.htaccess` rewrite) |
| **Dev Server** | PHP Built-in Server |

### Alasan Pilihan Teknologi

- **Native PHP MVC** dipilih agar codebase tetap ringan, mudah di-debug, dan dapat berjalan di shared hosting mana pun tanpa instalasi Composer atau framework tambahan.
- **MySQLi** (bukan PDO) digunakan secara konsisten dengan prepared statements untuk mencegah SQL injection.
- **Bootstrap Icons** dipilih untuk konsistensi ikon tanpa overhead framework CSS penuh.
- **SweetAlert2** memberikan konfirmasi dialog yang lebih baik dibandingkan `alert()` bawaan browser, terutama untuk operasi destruktif (hapus data).

---

## 🗂️ Struktur Folder

<details>
<summary><strong>📁 Klik untuk melihat struktur lengkap</strong></summary>

```text
kampung_ketupat/
│
├── app/                            # Inti aplikasi (MVC)
│   ├── controllers/                # Controller (logika request)
│   │   ├── AdminController.php         # Dashboard admin
│   │   ├── AdminEventController.php    # CRUD event (admin)
│   │   ├── AdminGaleriController.php   # CRUD galeri (admin)
│   │   ├── AdminKritikController.php   # Moderasi kritik saran (admin)
│   │   ├── AdminUMKMController.php     # CRUD UMKM (admin)
│   │   ├── AuthController.php          # Login & logout
│   │   ├── BerandaController.php       # Landing page
│   │   ├── EventController.php         # Halaman event publik
│   │   ├── GaleriController.php        # Halaman galeri publik
│   │   ├── KontakController.php        # Halaman kontak
│   │   ├── KritikSaranController.php   # Form kritik saran publik
│   │   ├── LokasiController.php        # Halaman lokasi
│   │   ├── UMKMController.php          # Halaman UMKM publik
│   │   └── WisataController.php        # Halaman wisata
│   │
│   ├── core/                       # Komponen inti framework
│   │   ├── Controller.php              # Base controller (view renderer)
│   │   ├── Csrf.php                    # CSRF token generator & validator
│   │   ├── ErrorHandler.php            # Global error handler
│   │   ├── LoginThrottle.php           # Brute-force protection
│   │   ├── Model.php                   # Base model (koneksi DB)
│   │   ├── Router.php                  # HTTP router (GET & POST)
│   │   └── SecurityLogger.php          # Security event logger (JSON)
│   │
│   ├── helpers/
│   │   └── upload.php                  # Validasi & pemrosesan upload gambar
│   │
│   ├── models/                     # Model (query database)
│   │   ├── AdminModel.php              # Query statistik dashboard
│   │   ├── EventModel.php              # Query tabel event
│   │   ├── GaleriModel.php             # Query tabel galeri
│   │   ├── KritikSaranModel.php        # Query tabel kritik_saran
│   │   └── UMKMModel.php               # Query tabel umkm
│   │
│   └── views/                      # Template HTML (PHP view)
│       ├── admin/
│       │   ├── dashboard.php
│       │   ├── layouts/
│       │   │   ├── header.php
│       │   │   ├── footer.php
│       │   │   └── main.php
│       │   ├── event/         (index, create, edit)
│       │   ├── galeri/        (index, create, edit)
│       │   ├── kritik_saran/  (index)
│       │   └── umkm/          (index, create, edit)
│       │
│       └── user/
│           ├── layouts/
│           │   ├── header.php
│           │   ├── footer.php
│           │   └── main.php
│           ├── beranda/       (index)
│           ├── event/         (index)
│           ├── galeri/        (index)
│           ├── kontak/        (index)
│           ├── kritik_saran/  (index)
│           ├── lokasi/        (index)
│           ├── umkm/          (index)
│           ├── wisata/        (detail)
│           └── errors/        (404, 500)
│
├── auth/
│   └── login.php                   # View halaman login admin
│
├── config/
│   └── database.php                # Konfigurasi koneksi DB + auto-init + seed
│
├── database/
│   └── kampung_ketupat.sql         # SQL schema alternatif (template kosong)
│
├── public/                         # Document root (hanya folder ini yang publik)
│   ├── index.php                       # Entry point utama aplikasi
│   ├── .htaccess                        # Rewrite rule untuk Apache
│   └── assets/
│       ├── css/
│       │   ├── style.css               # Stylesheet halaman publik
│       │   └── admin.css               # Stylesheet panel admin
│       ├── js/
│       │   ├── app.js                  # JS utama
│       │   ├── main.js                 # JS halaman publik
│       │   └── swal-helper.js          # Helper SweetAlert2
│       ├── images/
│       │   └── hero-ketupat.png        # Gambar hero/banner
│       └── uploads/
│           ├── event/                  # Upload foto event
│           ├── galeri/                 # Upload foto galeri
│           └── umkm/                   # Upload foto UMKM
│
├── routes/
│   └── web.php                     # Definisi seluruh route aplikasi
│
├── storage/
│   └── logs/                       # Log keamanan harian (JSON per baris)
│       └── security-YYYY-MM-DD.log
│
├── .gitignore
├── .htaccess                       # Redirect semua request ke public/
├── index.php                       # Redirect fallback ke public/
├── kampung_ketupat.sql             # SQL dump data terbaru (gunakan ini)
└── README.md
```

</details>

---

## 🏗️ Arsitektur Aplikasi

Aplikasi ini menggunakan pola **MVC sederhana berbasis native PHP** tanpa dependency eksternal. Berikut alur kerja request dari browser ke response:

```
Browser Request (HTTP GET/POST)
        │
        ▼
  public/.htaccess
  (Rewrite semua request → public/index.php)
        │
        ▼
  public/index.php
  (Define BASE_PATH, BASE_URL, load config & core)
        │
        ▼
  app/core/Router.php
  (Match URL + method → Controller@method)
        │
        ▼
  app/controllers/XxxController.php
  (Validasi CSRF, panggil Model, siapkan data)
        │
        ├──── app/models/XxxModel.php
        │     (Query MySQL via MySQLi prepared statement)
        │
        ▼
  app/views/user|admin/xxx/yyy.php
  (Render HTML dengan data dari controller)
        │
        ▼
  Response HTML ke Browser
```

### Komponen Inti

| Komponen | File | Peran |
|---|---|---|
| **Router** | `app/core/Router.php` | Mapping URL + HTTP method ke Controller@method. Menangani 404 otomatis. |
| **Base Controller** | `app/core/Controller.php` | Helper `render($view, $data)` untuk memanggil view dengan data. |
| **Base Model** | `app/core/Model.php` | Akses koneksi `$koneksi` (MySQLi) ke semua model. |
| **CSRF** | `app/core/Csrf.php` | Generate token 64-hex acak per sesi; validasi via `hash_equals()`. |
| **Login Throttle** | `app/core/LoginThrottle.php` | Lacak percobaan login per IP+username di tabel `auth_login_attempts`. |
| **Security Logger** | `app/core/SecurityLogger.php` | Tulis log JSON ke `storage/logs/security-YYYY-MM-DD.log`. |
| **Error Handler** | `app/core/ErrorHandler.php` | Tangani exception global; render halaman error 500. |

---

## 🗃️ Skema Database

Database bernama `kampung_ketupat` terdiri dari 6 tabel utama. Koneksi menggunakan **charset `utf8mb4`** (mendukung emoji dan karakter Unicode penuh).

### Tabel `admin`
Menyimpan akun pengelola website.

| Kolom | Tipe | Keterangan |
|---|---|---|
| `id` | INT AUTO_INCREMENT | Primary key |
| `username` | VARCHAR(100) UNIQUE | Username login |
| `password` | VARCHAR(255) | Hash bcrypt (`PASSWORD_DEFAULT`) |
| `nama_lengkap` | VARCHAR(150) | Nama tampil di dashboard |
| `created_at` | TIMESTAMP | Waktu pembuatan akun |

### Tabel `galeri`
Menyimpan foto-foto koleksi wisata.

| Kolom | Tipe | Keterangan |
|---|---|---|
| `id` | INT AUTO_INCREMENT | Primary key |
| `judul` | VARCHAR(200) | Judul foto |
| `deskripsi` | TEXT | Keterangan foto |
| `foto` | VARCHAR(255) | Path file atau URL gambar |
| `kategori` | ENUM | `wisata`, `kuliner`, `budaya`, `fasilitas`, `umum` |
| `is_publish` | TINYINT(1) | `1` = tampil publik, `0` = disembunyikan |
| `created_at` | TIMESTAMP | Waktu unggah |

### Tabel `event`
Menyimpan informasi kegiatan / event Kampung Ketupat.

| Kolom | Tipe | Keterangan |
|---|---|---|
| `id` | INT AUTO_INCREMENT | Primary key |
| `nama_event` | VARCHAR(200) | Nama kegiatan |
| `deskripsi` | TEXT | Penjelasan event |
| `tanggal_mulai` | DATE | Tanggal mulai |
| `tanggal_selesai` | DATE | Tanggal selesai |
| `jam_mulai` | TIME | Jam mulai |
| `jam_selesai` | TIME | Jam selesai |
| `lokasi` | VARCHAR(255) | Tempat pelaksanaan |
| `foto` | VARCHAR(255) | Path foto event |
| `status` | ENUM | `akan_datang`, `berlangsung`, `selesai` |
| `link_info` | VARCHAR(255) | Link informasi tambahan (opsional) |
| `created_at` | TIMESTAMP | Waktu input |

### Tabel `umkm`
Menyimpan data usaha mikro kecil menengah lokal.

| Kolom | Tipe | Keterangan |
|---|---|---|
| `id` | INT AUTO_INCREMENT | Primary key |
| `nama_umkm` | VARCHAR(200) | Nama usaha |
| `pemilik` | VARCHAR(150) | Nama pemilik/pengelola |
| `kategori` | ENUM | `kuliner`, `kerajinan`, `souvenir`, `jasa`, `lainnya` |
| `deskripsi` | TEXT | Deskripsi usaha |
| `produk_unggulan` | VARCHAR(255) | Produk/layanan andalan |
| `kontak` | VARCHAR(100) | No. HP / WhatsApp |
| `alamat` | VARCHAR(255) | Alamat lengkap |
| `foto` | VARCHAR(255) | Path foto usaha/produk |
| `created_at` | TIMESTAMP | Waktu input |

### Tabel `kritik_saran`
Menyimpan pesan masukan dari pengunjung.

| Kolom | Tipe | Keterangan |
|---|---|---|
| `id` | INT AUTO_INCREMENT | Primary key |
| `nama_pengunjung` | VARCHAR(150) | Nama pengirim |
| `email` | VARCHAR(150) | Email pengirim |
| `jenis` | ENUM | `kritik`, `saran`, `pertanyaan`, `apresiasi` |
| `pesan` | TEXT | Isi pesan |
| `sudah_dibaca` | TINYINT(1) | Flag sudah dibaca admin |
| `status` | ENUM | `pending`, `diterima`, `publik` |
| `tampil_mulai` | DATE | Tanggal mulai tampil (jika publik) |
| `tampil_selesai` | DATE | Tanggal selesai tampil |
| `created_at` | TIMESTAMP | Waktu pengiriman |

### Tabel `auth_login_attempts`
Melacak percobaan login untuk proteksi brute-force.

| Kolom | Tipe | Keterangan |
|---|---|---|
| `id` | INT AUTO_INCREMENT | Primary key |
| `ip_address` | VARCHAR(45) | Alamat IP (mendukung IPv6) |
| `username` | VARCHAR(100) | Username yang dicoba |
| `attempts` | INT | Jumlah percobaan gagal |
| `first_attempt_at` | DATETIME | Percobaan pertama |
| `last_attempt_at` | DATETIME | Percobaan terakhir |
| `blocked_until` | DATETIME NULL | Sampai kapan diblokir |

> **Index:** `UNIQUE(ip_address, username)` dan `INDEX(blocked_until)` untuk query cepat.

---

## 🧭 Halaman & Route Website

### Route Publik

| Method | URL | Controller@Method | Deskripsi |
|---|---|---|---|
| `GET` | `/` | `BerandaController@index` | Landing page utama |
| `GET` | `/galeri` | `GaleriController@index` | Halaman galeri foto |
| `GET` | `/event` | `EventController@index` | Daftar event |
| `GET` | `/umkm` | `UMKMController@index` | Daftar UMKM |
| `GET` | `/wisata` | `WisataController@index` | Info wisata |
| `GET` | `/lokasi` | `LokasiController@index` | Lokasi & peta |
| `GET` | `/kontak` | `KontakController@index` | Halaman kontak |
| `GET` | `/kritik-saran` | `KritikSaranController@index` | Form kritik & saran |
| `POST` | `/kritik-saran` | `KritikSaranController@index` | Submit form |

### Route Admin – Autentikasi

| Method | URL | Controller@Method | Deskripsi |
|---|---|---|---|
| `GET` | `/admin/login` | `AuthController@login` | Tampil form login |
| `POST` | `/admin/login/proses` | `AuthController@proses` | Proses autentikasi |
| `POST` | `/admin/logout` | `AuthController@logout` | Logout sesi |

### Route Admin – Dashboard

| Method | URL | Controller@Method | Deskripsi |
|---|---|---|---|
| `GET` | `/admin/dashboard` | `AdminController@dashboard` | Halaman utama admin |

### Route Admin – Galeri

| Method | URL | Deskripsi |
|---|---|---|
| `GET` | `/admin/galeri` | Daftar foto |
| `GET` | `/admin/galeri/create` | Form tambah foto |
| `POST` | `/admin/galeri/store` | Simpan foto baru |
| `GET` | `/admin/galeri/edit` | Form edit foto |
| `POST` | `/admin/galeri/update` | Update data foto |
| `POST` | `/admin/galeri/delete` | Hapus foto |
| `POST` | `/admin/galeri/togglePublish` | Toggle publish/unpublish |
| `POST` | `/admin/galeri/publishAll` | Publish semua foto |

### Route Admin – Event

| Method | URL | Deskripsi |
|---|---|---|
| `GET` | `/admin/event` | Daftar event |
| `GET` | `/admin/event/create` | Form tambah event |
| `POST` | `/admin/event/store` | Simpan event baru |
| `GET` | `/admin/event/edit` | Form edit event |
| `POST` | `/admin/event/update` | Update data event |
| `POST` | `/admin/event/delete` | Hapus event |

### Route Admin – UMKM

| Method | URL | Deskripsi |
|---|---|---|
| `GET` | `/admin/umkm` | Daftar UMKM |
| `GET` | `/admin/umkm/create` | Form tambah UMKM |
| `POST` | `/admin/umkm/store` | Simpan UMKM baru |
| `GET` | `/admin/umkm/edit` | Form edit UMKM |
| `POST` | `/admin/umkm/update` | Update data UMKM |
| `POST` | `/admin/umkm/delete` | Hapus UMKM |

### Route Admin – Kritik & Saran

| Method | URL | Deskripsi |
|---|---|---|
| `GET` | `/admin/kritik-saran` | Daftar pesan pending |
| `GET` | `/admin/kritik-saran/arsip` | Arsip pesan diproses |
| `POST` | `/admin/kritik-saran/terima` | Terima pesan |
| `POST` | `/admin/kritik-saran/tampilkan` | Jadikan publik |
| `POST` | `/admin/kritik-saran/sembunyikan` | Sembunyikan dari publik |
| `POST` | `/admin/kritik-saran/kembalikan` | Kembalikan ke pending |

---

## 🔐 Fitur Keamanan

Keamanan diimplementasikan secara berlapis (defence in depth):

### 1. CSRF Protection
- Setiap form POST menyertakan hidden field `_token` berisi token 64-karakter hex acak (`bin2hex(random_bytes(32))`).
- Token tersimpan di session dan divalidasi via `hash_equals()` (time-safe comparison) sebelum setiap operasi write.
- Token juga bisa dikirim via header `X-CSRF-TOKEN` untuk kompatibilitas AJAX.

### 2. Session Hardening
- `session_regenerate_id(true)` dipanggil setiap kali login berhasil untuk mencegah **session fixation attack**.
- Session ID lama dihapus secara eksplisit.

### 3. Login Throttle (Brute-Force Protection)
- Implementasi di `app/core/LoginThrottle.php` menggunakan tabel database `auth_login_attempts`.
- **Batas:** 5 percobaan gagal dalam window 10 menit.
- **Blokir:** IP + username diblokir selama 15 menit setelah melewati batas.
- Mendukung IPv6 (kolom `ip_address VARCHAR(45)`).
- Record lama (> 2 hari) otomatis dihapus saat inisialisasi.

### 4. Validasi Upload File
- Helper `app/helpers/upload.php` memvalidasi:
  - **MIME type** via `finfo_file()` (tidak hanya extension).
  - **Ukuran file** maksimum.
  - **Verifikasi gambar** via `getimagesize()`.
- File disimpan dengan nama acak (`{timestamp}_{random}`) untuk mencegah path traversal dan tebakan nama file.
- Folder upload diproteksi agar file PHP tidak bisa dieksekusi.

### 5. Route Destruktif via POST
- Semua operasi yang mengubah atau menghapus data (delete, update, toggle) **hanya bisa dilakukan via POST**, bukan GET.
- Mencegah penghapusan tidak disengaja melalui link prefetch browser atau crawler.

### 6. Security Logging
- Setiap kejadian penting (login gagal, controller tidak ditemukan, method tidak ada) dicatat oleh `SecurityLogger`.
- Format log: JSON per baris (`JSONL`) di `storage/logs/security-YYYY-MM-DD.log`.
- Setiap baris log berisi: `time`, `level`, `event`, `ip`, `method`, `uri`, `context`.

### 7. Blok Akses File Sensitif via `.htaccess`
- File `.htaccess` di root dan `public/` memastikan:
  - Semua request diarahkan ke `public/index.php`.
  - Folder `app/`, `config/`, `storage/`, `routes/` tidak dapat diakses langsung dari browser.
  - File `.env`, `.log`, `.sql` diblokir secara eksplisit.

### 8. Prepared Statements
- Seluruh query database menggunakan **MySQLi Prepared Statements** (`$stmt->bind_param()`).
- Tidak ada query dengan string interpolasi langsung — mencegah **SQL Injection** sepenuhnya.

---

## ⚙️ Konfigurasi Environment

Aplikasi mendukung konfigurasi via **environment variable** untuk deployment yang aman (nilai sensitif tidak perlu di-hardcode).

### Variabel yang Didukung

| Variabel | Default | Keterangan |
|---|---|---|
| `APP_ENV` | `local` | Mode aplikasi: `local` atau `production` |
| `DB_HOST` | `localhost` | Host server MySQL |
| `DB_USER` | `root` | Username database |
| `DB_PASS` | *(kosong)* | Password database |
| `DB_NAME` | `kampung_ketupat` | Nama database |
| `DB_CHARSET` | `utf8mb4` | Charset koneksi |
| `DB_AUTO_INIT` | `true` (lokal) | Auto-buat tabel jika belum ada |
| `DB_AUTO_SEED` | `true` (lokal) | Auto-isi data awal jika tabel kosong |

### Perilaku Per Mode

| Fitur | `local` | `production` |
|---|---|---|
| Auto-init tabel | ✅ | ❌ (import manual) |
| Auto-seed data awal | ✅ | ❌ |
| Error detail di browser | ✅ | ❌ (hanya di log) |

### Cara Set Environment Variable

**Linux/VPS:**
```bash
export APP_ENV=production
export DB_HOST=localhost
export DB_USER=dbuser
export DB_PASS=password_rahasia
export DB_NAME=kampung_ketupat
```

**Shared Hosting (via `.htaccess`):**
```apache
SetEnv APP_ENV production
SetEnv DB_HOST localhost
SetEnv DB_USER dbuser
SetEnv DB_PASS password_rahasia
SetEnv DB_NAME kampung_ketupat
```

---

## 🚀 Quick Start (Instalasi Lokal)

### Prasyarat

- PHP **8.2+** dengan ekstensi `mysqli`, `fileinfo`, `mbstring`
- MySQL **8.0+** atau MariaDB **10.6+**
- Apache atau PHP Built-in Server

### Langkah Instalasi

**1. Clone repository**

```bash
git clone https://github.com/kampungketupat/kampung_ketupat.git
cd kampung_ketupat
```

**2. Siapkan database**

Buat database baru di MySQL:

```sql
CREATE DATABASE kampung_ketupat CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
```

Import skema dan data:

```bash
# Gunakan file di root untuk data terbaru:
mysql -u root -p kampung_ketupat < kampung_ketupat.sql

# Atau gunakan template kosong (tanpa data):
mysql -u root -p kampung_ketupat < database/kampung_ketupat.sql
```

> **Catatan:** Jika menggunakan mode `local` dengan `DB_AUTO_INIT=true`, tabel akan otomatis dibuat dan data awal otomatis diisi saat pertama kali diakses.

**3. Konfigurasi koneksi (opsional)**

Jika konfigurasi default tidak sesuai, set environment variable sebelum menjalankan server.

**4. Jalankan server development**

```bash
# Menggunakan PHP built-in server (Windows - Laragon):
C:\laragon\bin\php\php-8.2.30-nts-Win32-vs16-x64\php.exe -S 127.0.0.1:8088 -t public

# Linux/macOS:
php -S 127.0.0.1:8088 -t public
```

**5. Akses di browser**

| URL | Keterangan |
|---|---|
| `http://127.0.0.1:8088/` | Halaman publik utama |
| `http://127.0.0.1:8088/admin/login` | Login panel admin |

**6. Kredensial default admin**

```
Username : admin
Password : admin123
```

> ⚠️ **Ganti password default segera** setelah login pertama kali, terutama sebelum deployment ke publik.

---

## 🌐 Deployment ke Hosting

Website ini sudah berhasil di-deploy di:

**🌐 [https://kampung-ketupat.infinityfree.me/](https://kampung-ketupat.infinityfree.me/)**

### Langkah Deployment ke Shared Hosting

**1. Upload file**

Upload seluruh isi folder proyek ke hosting melalui FTP/File Manager. Pastikan folder `public/` menjadi **Document Root** domain.

**2. Set Document Root**

Di cPanel, arahkan Document Root domain ke subfolder `public/` jika tersedia. Jika tidak bisa, pindahkan isi `public/` ke `public_html/` dan sesuaikan path di `index.php`.

**3. Import database**

Buat database di cPanel → MySQL Databases, lalu import `kampung_ketupat.sql` via **phpMyAdmin**.

**4. Set environment variable**

Tambahkan ke `.htaccess` di root:

```apache
SetEnv APP_ENV production
SetEnv DB_HOST localhost
SetEnv DB_USER nama_user_db
SetEnv DB_PASS password_db
SetEnv DB_NAME nama_database
```

**5. Set permission folder upload**

```bash
chmod 755 public/assets/uploads/
chmod 755 public/assets/uploads/galeri/
chmod 755 public/assets/uploads/event/
chmod 755 public/assets/uploads/umkm/
```

**6. Proteksi folder storage**

Pastikan `storage/logs/` tidak bisa diakses publik. Tambahkan `.htaccess` jika perlu:

```apache
# storage/logs/.htaccess
Deny from all
```

---

## 🧪 Testing & Smoke Test

### Syntax Check (PHP Lint)

```bash
# Cek entry point utama:
php -l public/index.php

# Cek konfigurasi database:
php -l config/database.php

# Cek semua file PHP sekaligus:
find . -name "*.php" -not -path "./public/assets/*" | xargs php -l
```

### Smoke Test Endpoint

Akses semua endpoint berikut dan pastikan tidak ada error:

| Endpoint | Ekspektasi |
|---|---|
| `/` | Halaman beranda tampil normal |
| `/galeri` | Grid foto tampil |
| `/event` | Daftar event tampil |
| `/umkm` | Daftar UMKM tampil |
| `/wisata` | Halaman wisata tampil |
| `/lokasi` | Halaman lokasi tampil |
| `/kontak` | Halaman kontak tampil |
| `/kritik-saran` | Form tampil, POST submit berhasil |
| `/admin/login` | Form login tampil |
| `/admin/dashboard` | Redirect ke login jika belum login |
| `/admin/galeri` | CRUD galeri berfungsi |
| `/admin/event` | CRUD event berfungsi |
| `/admin/umkm` | CRUD UMKM berfungsi |
| `/admin/kritik-saran` | Moderasi berfungsi |

### Cek File Log

```bash
# Lihat log keamanan hari ini:
cat storage/logs/security-$(date +%Y-%m-%d).log

# Format log (JSONL) - satu baris per event:
# {"time":"2026-04-28T...","level":"warning","event":"auth.login_fail","ip":"...","context":{...}}
```

---

## 📸 Screenshot Aplikasi

> Untuk melihat tampilan lengkap aplikasi secara visual, kunjungi:
>
> - 🌐 **Live Demo:** [kampung-ketupat.infinityfree.me](https://kampung-ketupat.infinityfree.me/)
> - 📊 **Slide Presentasi:** [Canva Deck](https://canva.link/54cr2ep7p6ouwdr)
> - 📄 **Laporan Lengkap:** [Google Drive](https://drive.google.com/drive/folders/1NnE_3vCfHOyXmjiId5lK8Y-TGkFcHNcU?usp=sharing)

---

## 📎 Dokumentasi Pendukung

| Dokumen | Tautan | Keterangan |
|---|---|---|
| 📑 Slide Presentasi | [Canva](https://canva.link/54cr2ep7p6ouwdr) | Deck presentasi proyek (Canva) |
| 📄 Laporan Proyek | [Google Drive](https://drive.google.com/drive/folders/1NnE_3vCfHOyXmjiId5lK8Y-TGkFcHNcU?usp=sharing) | Laporan lengkap pengembangan |
| 🎤 Rekaman Wawancara | [Google Drive](https://drive.google.com/drive/folders/1nMXrLRJ-9rJV7JU9HYuCDG_3R1cVz6eg?usp=sharing) | Hasil wawancara dengan stakeholder |
| 🗺️ Flowchart Sistem | [Draw.io](https://drive.google.com/file/d/1xvJ7Z_Qhu0zfzCXTjoyFLHQ2VosqakOO/view?usp=drive_link) | Diagram alur sistem & proses bisnis |

---

## 👥 Tim Pengembang

Proyek ini dikembangkan sebagai bagian dari kegiatan akademik / pengembangan komunitas untuk mendukung digitalisasi Kampung Ketupat.

> Untuk kontribusi, pertanyaan, atau laporan bug, silakan buka **Issue** di repository ini atau hubungi tim pengembang melalui informasi yang tersedia di halaman [Kontak](https://kampung-ketupat.infinityfree.me/kontak).

---

## 📜 Lisensi

Proyek ini dilisensikan di bawah **MIT License**.

```
MIT License — bebas digunakan, dimodifikasi, dan didistribusikan
dengan menyertakan atribusi kepada pengembang asli.
```

---

<div align="center">

Dibuat dengan ❤️ untuk Kampung Ketupat

[![Live](https://img.shields.io/badge/🌐_Live_Demo-kampung--ketupat.infinityfree.me-0d9488?style=for-the-badge)](https://kampung-ketupat.infinityfree.me/)

</div>
