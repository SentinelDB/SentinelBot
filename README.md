<div align="center">
  <img src="sentinel.jpg" alt="Sentinel Bot" width="200" height="200" style="border-radius: 20px;" />
  
  # Sentinel Bot
  
  ### Private Intelligence Services
  
  > Informasi adalah kekuasaan, dan kami memberi Anda aksesnya.
  
  [![Telegram](https://img.shields.io/badge/Telegram-%40SentinelUser__Bot-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/SentinelUser_Bot)
  [![GitHub stars](https://img.shields.io/github/stars/SentinelDB/SentinelBot?style=for-the-badge&logo=github&color=yellow)](https://github.com/SentinelDB/SentinelBot/stargazers)
  [![GitHub forks](https://img.shields.io/github/forks/SentinelDB/SentinelBot?style=for-the-badge&logo=github&color=blue)](https://github.com/SentinelDB/SentinelBot/network/members)
  [![GitHub issues](https://img.shields.io/github/issues/SentinelDB/SentinelBot?style=for-the-badge&logo=github&color=red)](https://github.com/SentinelDB/SentinelBot/issues)
  
  [Bot Telegram](https://t.me/SentinelUser_Bot) · [⭐ Beri Stars](https://github.com/SentinelDB/SentinelBot/stargazers) · [🐛 Report Bug](https://github.com/SentinelDB/SentinelBot/issues)
</div>

---

Sentinel Bot adalah platform Private Intelligence Services yang berjalan di atas Telegram Bot. Dibangun untuk melakukan pencarian, verifikasi, dan analisis informasi dari berbagai sumber digital secara cepat, terstruktur, dan bertanggung jawab.

---

## Daftar Isi

- [Tentang Sentinel Bot](#tentang-sentinel-bot)
- [Fitur Utama](#fitur-utama)
  - [Free Services](#free-services)
  - [Premium Services](#premium-services)
  - [Topup Limit](#topup-limit)
- [Cara Penggunaan](#cara-penggunaan)
  - [Memulai](#memulai)
  - [AUTO 1CLICK OSINT](#auto-1click-osint)
  - [Cek Nomor Hp](#cek-nomor-hp)
  - [Stalk Sosmed](#stalk-sosmed)
  - [Foto -> Identitas](#foto---identitas)
  - [Lacak Penipu](#lacak-penipu)
  - [Check & Top Up Limit](#check--top-up-limit)
- [Sistem Limit & Kuota](#sistem-limit--kuota)
- [AI Intelligence Summary](#ai-intelligence-summary)
- [Canvas Investigation Board](#canvas-investigation-board)
- [Disclaimer](#disclaimer)

---

## Tentang Sentinel Bot

Sentinel Bot mengkonsolidasikan kemampuan investigasi digital yang sebelumnya tersebar di puluhan tools berbeda — ke dalam satu antarmuka Telegram Bot yang sederhana namun powerful. Tidak perlu instalasi software. Tidak perlu technical skills. Cukup buka bot, pilih layanan, dan dapatkan hasil.

**Yang bisa dilakukan Sentinel Bot:**
- Mengumpulkan informasi dari berbagai sumber terbuka secara otomatis
- Menganalisis jejak digital individu maupun entitas
- Memberikan rangkuman intelligence berbasis AI untuk setiap hasil OSINT
- Menyajikan data dalam format yang actionable, bukan sekadar data mentah
- Menghasilkan laporan PDF untuk dokumentasi

---

## Fitur Utama

### Free Services

#### 🎯 AUTO 1CLICK OSINT

Pencarian informasi dari berbagai sumber terbuka dalam satu proses terintegrasi untuk mempercepat intelligence gathering.

Cukup masukkan nama, username, email, nomor telepon, domain, atau URL — Sentinel Bot akan:
1. **Deteksi entitas** — otomatis mengidentifikasi jenis data yang dimasukkan (nama, email, username, phone, domain, IP, NIK, NPWP, nomor rekening, plat nomor)
2. **Build search queries** — membuat query pencarian yang ditargetkan berdasarkan entitas yang terdeteksi (Multi-Search Engine, site-specific searches seperti LinkedIn/Facebook/Instagram/Telegram, filetype searches untuk PDF)
3. **Multi-source search** — menjalankan pencarian via Multi-Search Engine dengan fallback ke sumber alternatif
4. **AI Intelligence Summary** — setelah hasil dikumpulkan, AI membuat rangkuman intelligence dalam Bahasa Indonesia dengan struktur: Ringkasan Intelligence, Temuan Kunci, Penilaian Risiko, Rekomendasi Tindakan, dan Sumber Data
5. **Laporan PDF** — hasil lengkap dikemas dalam PDF report untuk dokumentasi

**Limit gratis:** 2x per hari (reset 00:00 WIB)

---

#### 📱 Cek Nomor Hp

Pemeriksaan nomor telepon untuk menampilkan informasi dasar yang tersedia: nama yang teridentifikasi, operator (carrier), negara asal nomor, serta status ketersediaan akun WhatsApp.

**Sumber data:**
- **Truecaller** — identifikasi nama pemilik nomor
- **WhatsApp Store** — cek apakah nomor terdaftar di WhatsApp, termasuk status business account
- **WhatsApp Business Profile** — ambil business profile jika nomor adalah akun business

**Format input:** `+<country code><nomor>`
- Indonesia: `+6281234567890`
- USA: `+14155552671`
- UK: `+447911123456`
- Jepang: `+819012345678`

**Limit gratis:** 2x per hari (reset 00:00 WIB)

---

#### 🔍 Stalk Sosmed

Analisis jejak dan aktivitas akun publik berdasarkan data yang tersedia di berbagai platform sosial media.

**Platform yang didukung:**

| Platform | Data yang Dikirim |
|----------|-------------------|
| **Telegram** | Foto profil, nama, bio, tipe akun (verified/public) |
| **TikTok** | Foto profil, stats (followers/following/likes/videos), recent posts (video MP4 + music MP3), following list (canvas board) |
| **X/Twitter** | Foto profil, banner, bio, lokasi, stats (posts/following/followers/likes), recent tweets (text + images + videos), following/followers list (canvas board) |
| **Instagram** | Foto profil HD, bio, external URL, stats (posts/following/followers/highlights/reels), recent posts (foto + video + carousel), stories (24h), highlights, canvas board followers/following/mutual |
| **Facebook** | Foto profil HD, cover photo, bio, stats (followers/likes/posts), recent posts, friends/following/followers list (canvas board), stories |

**Canvas Investigation Board:**
Setiap hasil stalk menghasilkan canvas board berupa file PNG yang dikirim sebagai document (HD quality) dengan layout investigasi:
- **Target** di tengah atas dengan foto profil
- **User nodes** tersebar dalam pola zigzag (kiri-kanan) dengan foto, nama, username, badge (Verified/Private)
- **Connection lines** dari target ke setiap user
- **3 user terbaru di-highlight** dengan ring
- Tema warna berbeda per platform: IG (merah/hijau/emas), FB (biru/hijau/ungu), TikTok (pink/cyan), Twitter (biru/ungu/hijau)

**Auto-Follow (Instagram):**
Jika target Instagram bersifat private, bot otomatis mengirim follow request. Setelah request diterima, bot akan re-stalk untuk mengambil semua data (posts, stories, highlights) tanpa membuat Case baru atau mengurangi limit harian.

**Limit gratis:** 2x per hari (reset 00:00 WIB)

---

### Premium Services

#### 📷👤 Foto -> Identitas

Pencocokan wajah terhadap jejak digital yang tersedia sebagai bagian dari proses investigasi.

User mengunggah foto (JPG/PNG), kemudian sistem melakukan analisis dan pencocokan wajah. Hasil dikirim ke admin untuk diproses secara manual.

**Cara pakai:**
1. Klik tombol **📷👤 Foto -> Identitas**
2. Unggah foto yang jelas
3. Konfirmasi
4. Bayar sesuai harga yang tertera
5. Upload bukti pembayaran
6. Admin memproses dan mengirim hasil

---

#### 🗺️ Lacak Penipu

Layanan pelacakan lokasi melalui mekanisme yang sah dan sesuai ketentuan yang berlaku.

User memberikan nomor telepon target, sistem membuat Case dan meneruskan ke admin untuk diproses.

**Cara pakai:**
1. Klik tombol **🗺️ Lacak Penipu**
2. Masukkan nomor telepon target (format: `+<country code><nomor>`)
3. Konfirmasi
4. Bayar sesuai harga yang tertera
5. Upload bukti pembayaran
6. Admin memproses dan mengirim hasil

---

### Topup Limit

#### 💰 Check & Top Up Limit

Beli tambahan kuota untuk fitur gratis (OSINT, Cek Nomor Hp, Stalk Sosmed) ketika limit harian habis.

**Cara kerja:**
- Purchased quota **TIDAK reset** saat pergantian hari (berbeda dengan daily free limit yang reset 00:00 WIB)
- Sistem menggunakan daily free limit (2x/hari) terlebih dahulu
- Jika daily limit habis, sistem otomatis menggunakan purchased quota
- Purchased quota hanya berkurang saat result **berhasil** (jika target tidak ditemukan, quota tidak berkurang)

**Pricing (dapat diatur admin via dashboard):**
- Harga default: Rp 1.000 per limit
- Minimal topup: 20 limit (Rp 20.000)
- Maksimal topup: 1.000.000 limit

**Cara pakai:**
1. Klik tombol **💰 Check & Top Up Limit**
2. Pilih service (🔍 Stalk Sosmed / 📱 Cek Nomor Hp / 🎯 AUTO 1CLICK OSINT)
3. Masukkan jumlah limit yang ingin dibeli
4. Konfirmasi — invoice dibuat
5. Scan QRIS yang dikirim bot untuk pembayaran
6. Upload bukti pembayaran
7. Admin approve → quota otomatis ditambahkan ke akun Anda
8. Anda mendapat notifikasi "Topup Berhasil"

---

## Cara Penggunaan

### Memulai

1. Buka Telegram, cari **[@SentinelUser_Bot](https://t.me/SentinelUser_Bot)**
2. Ketik `/start`
3. Pada pertama kali, Anda akan diminta verifikasi captcha (matematika sederhana, 1x saja per akun)
4. Setelah verifikasi, menu utama akan muncul dengan 6 tombol:

```
┌─────────────────────────────┐
│  🎯 AUTO 1CLICK OSINT       │
├─────────────────────────────┤
│  🗺️ Lacak Penipu            │
├─────────────────────────────┤
│  📷👤 Foto -> Identitas      │
├─────────────────────────────┤
│  📱 Cek Nomor Hp            │
├─────────────────────────────┤
│  🔍 Stalk Sosmed            │
├─────────────────────────────┤
│  💰 Check & Top Up Limit    │
└─────────────────────────────┘
```

### AUTO 1CLICK OSINT

1. Klik **🎯 AUTO 1CLICK OSINT**
2. Bot meminta target — ketik nama, username, email, nomor telepon, domain, atau URL
3. Tunggu countdown 10 detik (anti-spam)
4. OSINT engine berjalan (5-15 detik)
5. Hasil dikirim ke chat Anda:
   - **OSINT Report** — daftar entitas terdeteksi + hasil pencarian per query
   - **PDF Report** — laporan lengkap untuk dokumentasi
   - **AI Intelligence Summary** — rangkuman intelligence dalam Bahasa Indonesia
6. Jika tidak ada entitas terdeteksi, quota tidak berkurang

### Cek Nomor Hp

1. Klik **📱 Cek Nomor Hp**
2. Bot meminta nomor telepon — ketik dalam format internasional (`+62...`, `+1...`, dll)
3. Tunggu countdown 10 detik
4. Hasil dikirim: nama, carrier, negara, status WhatsApp
5. Jika nomor tidak ditemukan (nama "Tidak diketahui"), quota tidak berkurang

### Stalk Sosmed

1. Klik **🔍 Stalk Sosmed**
2. Pilih platform (Telegram, TikTok, X/Twitter, Instagram, Facebook)
3. Bot meminta username — ketik tanpa `@`
4. Tunggu countdown 10 detik
5. Hasil dikirim sesuai platform:
   - Foto profil HD
   - Info profil (nama, bio, stats)
   - Recent posts (foto, video, carousel)
   - Stories (jika akun public)
   - Highlights (Instagram)
   - Canvas board (followers/following/friends — sebagai document PNG HD)
6. Jika username tidak ditemukan, quota tidak berkurang

### Foto -> Identitas

1. Klik **📷👤 Foto -> Identitas**
2. Upload foto yang jelas (JPG/PNG)
3. Klik **Lanjutkan**
4. Bayar sesuai harga (QRIS dikirim bot)
5. Upload bukti pembayaran
6. Admin verifikasi → proses → hasil dikirim ke chat Anda

### Lacak Penipu

1. Klik **🗺️ Lacak Penipu**
2. Masukkan nomor telepon target
3. Klik **Lanjutkan**
4. Bayar sesuai harga (QRIS dikirim bot)
5. Upload bukti pembayaran
6. Admin verifikasi → proses → hasil dikirim ke chat Anda

### Check & Top Up Limit

1. Klik **💰 Check & Top Up Limit**
2. Bot menampilkan: harga per limit, minimal/maksimal topup, saldo purchased quota Anda
3. Pilih service (🔍 Stalk Sosmed / 📱 Cek Nomor Hp / 🎯 AUTO 1CLICK OSINT)
4. Masukkan jumlah limit (angka)
5. Konfirmasi — invoice + QRIS dikirim
6. Scan QRIS → bayar → upload bukti
7. Admin approve → quota aktif langsung

---

## Sistem Limit & Kuota

Sentinel Bot menggunakan sistem dual-quota:

| Tipe | Reset | Cara Dapat |
|------|-------|------------|
| **Daily Free Limit** | Reset 00:00 WIB setiap hari | Otomatis untuk semua user |
| **Purchased Quota** | TIDAK reset (permanen sampai habis) | Beli via Topup Limit |

**Prioritas pemakaian:**
1. Daily free limit dipakai duluan (2x/hari)
2. Jika daily limit habis → otomatis pakai purchased quota
3. Purchased quota di-decrement HANYA saat result berhasil

**Anti-waste policy:**
Jika hasil tidak ditemukan (username tidak ada / nomor tidak teridentifikasi / OSINT tidak menemukan entitas), case dihapus dari database dan quota **TIDAK berkurang** — baik daily maupun purchased.

---

## AI Intelligence Summary

Setiap hasil OSINT yang memiliki entitas terdeteksi akan otomatis mendapat rangkuman AI dari Sentinel-AI service (powered by Ollama — nemotron-3-nano:30b-cloud).

**Struktur rangkuman:**
- **Ringkasan Intelligence** — paragraf pembuka tentang target dan eksposur
- **Temuan Kunci** — bullet list temuan konkret dengan kategori (Jejak Digital, Eksposur Identitas, Informasi Kontak, dll)
- **Penilaian Risiko** — bullet list area dengan tingkat eksposur (Rendah/Sedang/Tinggi)
- **Rekomendasi Tindakan** — 3-5 rekomendasi konkret
- **Sumber Data** — daftar sumber yang dianalisis

Bahasa: Full Bahasa Indonesia formal, tegas, presisi.

---

## Canvas Investigation Board

Untuk fitur Stalk Sosmed, hasil followers/following/friends ditampilkan sebagai canvas board PNG (HD quality, dikirim sebagai document):

**Layout:**
- Target di tengah atas dengan foto profil + glow effect
- User nodes tersebar zigzag (kiri-kanan alternatif)
- Connection lines (bezier curves) dari target ke setiap user
- 3 user terbaru di-highlight dengan ring
- Badge: `[V]` = Verified, `[P]` = Private
- Grid background dengan tema dark
- Footer dengan total count + branding

**Tema warna per platform:**
- Instagram: Followers (merah `#e94560`), Following (hijau `#4ecca3`), Mutual (emas `#f5a623`)
- Facebook: Friends (biru `#1877F2`), Following (hijau `#4ecca3`), Followers (ungu `#9b59b6`)
- TikTok: Following (pink `#FE2C55`), Engaged Viewers (cyan `#25F4EE`)
- Twitter: Following (biru `#1DA1F2`), Followers (ungu `#5D5FEF`), Engaged Accounts (hijau `#00BA7C`)

---

## Disclaimer

Sentinel Bot adalah platform yang menyediakan akses ke informasi dari sumber terbuka (Open Source Intelligence). Seluruh data yang ditampilkan bersumber dari informasi publik yang dapat diakses oleh siapa pun.

Penggunaan Sentinel Bot tunduk pada ketentuan berikut:
- Setiap layanan hanya untuk tujuan lawful & legitimate
- Pengguna bertanggung jawab atas penggunaan data yang diperoleh
- Platform tidak menyimpan data hasil investigasi selain untuk log audit
- Setiap layanan tunduk pada ketentuan penggunaan platform

---

<div align="center">

**Sentinel Bot** — Private Intelligence Services

Informasi adalah kekuasaan, dan kami memberi Anda aksesnya.

[![Telegram](https://img.shields.io/badge/Telegram-%40SentinelUser__Bot-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/SentinelUser_Bot)
[![GitHub stars](https://img.shields.io/github/stars/SentinelDB/SentinelBot?style=for-the-badge&logo=github&color=yellow)](https://github.com/SentinelDB/SentinelBot/stargazers)

⭐ Jangan lupa beri Stars di [GitHub](https://github.com/SentinelDB/SentinelBot) jika bot ini bermanfaat!

</div>
