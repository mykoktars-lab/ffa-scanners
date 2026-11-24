# FFA Smart Scanner

Aplikasi web/PWA untuk membantu membaca catatan dua kolom, menghitung FFA, dan mengekspor tabel hasil sebagai gambar PNG.

## Isi project

- `index.html` — tampilan, input data, OCR, kalkulasi, dan ekspor gambar.
- `manifest.json` — identitas dan konfigurasi instalasi PWA.
- `sw.js` — service worker untuk cache app shell.
- `assets/icon.svg` — ikon aplikasi.
- `.nojekyll` — menonaktifkan pemrosesan Jekyll di GitHub Pages.
- `.github/workflows/deploy.yml` — workflow deployment GitHub Pages.
- `LICENSE` — lisensi project.

## Rumus

`FFA (%) = Volume titrasi (mL) × Normalitas NaOH × Faktor asam oleat ÷ Berat sampel (g)`

Parameter awal:
- Faktor asam oleat: `25.6`
- Normalitas NaOH: `0.0429`

Parameter dapat diubah dari aplikasi. Pastikan sesuai metode/SOP laboratorium.

## Cara memasang di GitHub Pages

1. Buat repository GitHub baru, misalnya `ffa-smart-scanner`.
2. Ekstrak ZIP ini di komputer/HP.
3. Unggah seluruh isi folder project ke root repository (termasuk folder `.github` dan `assets`).
4. Buka **Settings → Pages**.
5. Pada **Build and deployment**, pilih **GitHub Actions**.
6. Buka tab **Actions**, jalankan workflow jika belum berjalan.
7. Setelah deployment selesai, buka URL GitHub Pages yang ditampilkan GitHub.
8. Di Android Chrome, buka menu browser lalu pilih **Tambahkan ke layar utama** atau **Install app** jika tersedia.

## Catatan OCR yang penting

Versi ini menggunakan Tesseract.js melalui CDN. Perlu koneksi internet untuk memuat library OCR. Pengenalan tulisan tangan dan tata letak dua kolom tidak dijamin akurat. Implementasi awal mengambil angka yang dikenali sesuai urutan teks dan memasangkannya berurutan; aplikasi belum memahami batas kolom secara andal.

**Wajib cocokkan setiap angka dengan foto sumber sebelum menekan Hitung FFA.** Jika OCR keliru, edit angka pada tabel. Untuk hasil lebih baik, foto tegak lurus, terang, fokus, dan minim bayangan.

## Catatan PWA/offline

Service worker menyimpan app shell setelah kunjungan pertama. OCR memakai library eksternal CDN dan mungkin tidak tersedia saat offline. Kamera, install prompt, dan berbagi file bergantung pada dukungan browser serta konteks HTTPS.

## Verifikasi

Aplikasi ini alat bantu perhitungan, bukan pengganti SOP, pemeriksaan analis, atau validasi laboratorium. Periksa parameter, satuan, data mentah, dan hasil sebelum digunakan sebagai data resmi.


## V3 Premium update
- Premium visual theme with cinematic 5-second intro video (`assets/intro.mp4`).
- Guest entry screen; no password or account system is required. Guest mode is a local front-end entry only, not secure authentication.
- Optional ambient background sound synthesized by the browser after the user taps the guest button. It can be switched off.
- Existing FFA calculation, OCR, editable rows, and PNG report export are retained.
- Replace the repository files with the contents of this ZIP to publish V3. Keep the `.github/workflows/deploy.yml` file.
