# TravelKu — myBCA Prototype

Prototype single-page HTML untuk TravelKu (myBCA). User demo: **Dina Mika**. Asisten AI: **Fadhil AI**.

## Yang ada di revisi ini
- **True mobile viewport** — bukan lagi mockup HP di tengah desktop. App sekarang full-screen (100dvh/100vw) begitu dibuka di HP, lengkap dengan `env(safe-area-inset-*)` biar aman dari notch & home-indicator.
- **Alur myBCA → TravelKu** tetap dipertahankan: buka app dari layar myBCA Home, ketuk kartu TravelKu untuk masuk.
- **Header brand TravelKu** (logo mark + wordmark) muncul konsisten di layar dashboard.
- **Fadhil AI** — asisten AI di pojok kiri bawah, avatar berubah outfit begitu masuk TravelKu, bisa diajak chat.
- **Tur panduan in-app** — muncul otomatis untuk pengguna baru (setelah popup promo pertama), highlight TravelKu, Wallet, Explore, Fadhil AI, dan Rewards/Split Bill. Bisa diulang kapan saja lewat menu **More → Tur Panduan**.
- Semua fitur lama (Wallet, Explore, Stats, Split Bill, Reward Center, Ringkasan, Notifikasi, Mode Darurat) tetap utuh — tidak ada yang dihapus.
- Split Bill sekarang juga mendukung metode bayar **OVO**.

## Catatan jujur soal scope
- Logo di header masih pakai logomark bikinan sendiri (kotak biru "B"/"T") karena belum ada file PNG logo asli yang diupload ke chat ini. Begitu kamu upload PNG logonya, aku bisa langsung pasang di posisi yang sama.
- Project ini tetap murni HTML/CSS/JS satu file (tanpa Vite/React/PWA config) karena metode deploy-nya GitHub Pages statis — itu paling stabil dan tidak butuh proses build sama sekali. Kalau ke depannya kamu mau versi berbasis Vite/PWA installable, bilang aja, itu proyek terpisah.

## Cara Deploy ke GitHub Pages

1. Buat repository baru di GitHub (public), misalnya `travelku-prototype`.
2. Upload/push semua isi folder ini (termasuk `index.html`) ke repo tersebut.
3. Di repo, buka **Settings > Pages**.
4. Pada bagian **Branch**, pilih `main` (atau branch tempat kamu push) dan folder `/root`, lalu klik **Save**.
5. Tunggu 1–2 menit, lalu situs akan aktif di:
   `https://<username-kamu>.github.io/<nama-repo>/`

## Cara Deploy via Git CLI (opsional, lebih cepat)

```bash
git init
git add .
git commit -m "Initial commit - TravelKu prototype"
git branch -M main
git remote add origin https://github.com/<username-kamu>/<nama-repo>.git
git push -u origin main
```

Setelah itu tinggal aktifkan GitHub Pages seperti langkah di atas.

## Catatan

- File utama sudah diberi nama `index.html` supaya otomatis terbaca sebagai halaman utama oleh GitHub Pages.
- Tidak ada dependency build (murni HTML/CSS/JS + CDN), jadi tidak perlu proses instalasi apa pun.
