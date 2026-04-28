# ✨ Sayid Rafi A'thaya — Portfolio ✨

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
