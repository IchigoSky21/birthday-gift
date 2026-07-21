<div align="center">
# 🎂 Birthday Card Generator
### ✨ Ucapan ulang tahun interaktif yang bisa digunakan untuk siapa saja ✨
<br/>
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[🔗 Live Demo](https://ichigosky21.github.io/birthday-gift/) · [🐛 Report Bug](https://github.com/IchigoSky21/birthday-gift/issues)
</div>
---
## 📖 Tentang Project
**Birthday Card Generator** adalah kartu ucapan ulang tahun digital yang interaktif dan penuh animasi. Cukup masukkan **nama** dan **usia** penerima, maka kartu unik akan dihasilkan secara otomatis — lengkap dengan tema warna random, musik latar, dan animasi yang memukau.
> 💡 Dibuat sebagai hadiah personal, tapi bisa digunakan oleh siapa saja untuk siapa saja!
---
## 🎮 Cara Kerja
```
📝 Input Nama & Usia  →  🚪 Animasi Pintu & Kunci  →  🏅 Badge & Ucapan  →  🎵 Musik Otomatis
```
|
 Step 
|
 Aksi 
|
|
------
|
------
|
|
**
1
**
|
 Masukkan 
**
nama
**
 dan 
**
usia
**
 penerima di form input 
|
|
**
2
**
|
 Klik kunci 🔑 untuk membuka pintu dengan animasi 
|
|
**
3
**
|
 Lihat badge medali dengan usia dan confetti 🎊 
|
|
**
4
**
|
 Klik tombol untuk membuka surat ucapan 
|
|
**
5
**
|
 Nikmati musik latar yang diputar otomatis 🎵 
|
---
## ✨ Fitur
- 🎨 **5 Tema Warna Random** — Teal & Gold, Purple Dream, Midnight Rose, Forest Glow, Sunset Blaze
- 🎵 **Musik Random** — 4 lagu siap putar dengan mini player bergaya Spotify (vinyl spin, progress bar, equalizer)
- 🚪 **Animasi Pintu Interaktif** — Pintu terbuka dengan animasi smooth saat kunci diklik
- 🏅 **Badge Medali** — Menampilkan usia dengan desain medali emas yang elegan
- 🎊 **Confetti & Floating Emoji** — Hujan confetti berwarna-warni sesuai tema
- 📝 **Surat Ucapan** — Pesan birthday dengan sentuhan Korea (생일 축하해!)
- 🔊 **UI Sound Effects** — Efek suara kecil saat interaksi (Web Audio API)
- 📸 **Download as Image** — Simpan kartu sebagai gambar PNG
- ♿ **Accessible** — Keyboard navigation & ARIA labels
- 📱 **Responsive** — Tampil sempurna di mobile & desktop
---
## 🎵 Playlist
|
#
|
 Lagu 
|
 Artis 
|
 Mulai dari 
|
|
---
|
------
|
-------
|
-----------
|
|
 1 
|
 Monokrom 
|
 Tulus 
|
 0:30 
|
|
 2 
|
 Just The Way You Are 
|
 Bruno Mars 
|
 0:16 
|
|
 3 
|
 OMG 
|
 NewJeans 
|
 0:45 
|
|
 4 
|
 APT 
|
 ROSÉ & Bruno Mars 
|
 0:00 
|
> 🎶 Lagu dipilih secara **random** setiap kali kartu dibuat!
---
## 🎨 Tema Warna
|
 Tema 
|
 Preview 
|
|
------
|
---------
|
|
**
Teal & Gold
**
|
 🟡🟠🟢 
|
|
**
Purple Dream
**
|
 🟣💜💗 
|
|
**
Midnight Rose
**
|
 🩷🌹🔵 
|
|
**
Forest Glow
**
|
 🟢💚🩵 
|
|
**
Sunset Blaze
**
|
 🟠🔴🔵 
|
---
## 🚀 Cara Pakai
### Langsung Buka
Cukup kunjungi link live demo atau buka file `index.html` di browser:
```bash
# Clone repository
git clone https://github.com/IchigoSky21/birthday-gift.git
# Masuk ke folder
cd birthday-gift
# Buka di browser
start index.html        # Windows
open index.html         # macOS
xdg-open index.html     # Linux
```
### Menambah Lagu Baru
Edit array `PLAYLIST` di dalam `index.html`:
```javascript
const PLAYLIST = [
  { file: 'monokrom.mp3', title: 'Monokrom', artist: 'Tulus', startAt: 30 },
  { file: 'lagu-baru.mp3', title: 'Judul Lagu', artist: 'Artis', startAt: 0 },
  // Tambahkan lagu lainnya di sini...
];
```
> ⚠️ Letakkan file `.mp3` di folder yang sama dengan `index.html`
---
## 📁 Struktur File
```
birthday-gift/
├── index.html          # Aplikasi utama (HTML + CSS + JS)
├── monokrom.mp3        # 🎵 Tulus - Monokrom
├── jtwya.mp3           # 🎵 Bruno Mars - Just The Way You Are
├── omg.mp3             # 🎵 NewJeans - OMG
├── apt.mp3             # 🎵 ROSÉ & Bruno Mars - APT
└── README.md           # Dokumentasi
```
---
## 🛠️ Tech Stack
- **HTML5** — Struktur & semantik
- **CSS3** — Styling, animasi, glassmorphism, backdrop-filter
- **Vanilla JavaScript** — Logika, Web Audio API, DOM manipulation
- **Google Fonts** — Fredoka & Karla
- **html2canvas** — Screenshot / download kartu sebagai gambar (CDN)
> 🎯 **Zero dependencies** — Tidak perlu install apapun. Cukup buka di browser!
---
## 📱 Browser Support
|
 Browser 
|
 Status 
|
|
---------
|
--------
|
|
 Chrome 90+ 
|
 ✅ Fully Supported 
|
|
 Firefox 90+ 
|
 ✅ Fully Supported 
|
|
 Safari 15+ 
|
 ✅ Fully Supported 
|
|
 Edge 90+ 
|
 ✅ Fully Supported 
|
|
 Mobile Chrome 
|
 ✅ Fully Supported 
|
|
 Mobile Safari 
|
 ✅ Fully Supported 
|
---
## 🤝 Kontribusi
Kontribusi sangat diterima! Silakan:
1. **Fork** repository ini
2. Buat **branch** baru (`git checkout -b fitur-baru`)
3. **Commit** perubahan (`git commit -m 'Tambah fitur baru'`)
4. **Push** ke branch (`git push origin fitur-baru`)
5. Buat **Pull Request**
---
## 📄 Lisensi
Project ini dibuat dengan ❤️ untuk tujuan personal. Silakan gunakan dan modifikasi sesuai kebutuhan.
---
<div align="center">
**Made with ❤️ by [IchigoSky21](https://github.com/IchigoSky21)**
🎂 *Selamat ulang tahun untuk siapapun yang menerima kartu ini!* 🎂
</div>
