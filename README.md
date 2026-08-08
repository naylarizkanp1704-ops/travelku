# TravelKu — myBCA Prototype

Prototype single-page HTML untuk TravelKu (myBCA).

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
