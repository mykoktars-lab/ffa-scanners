# FFA Smart Scanner V4

- Intro video dari pengguna (10 detik), tombol LEWATI di tengah bawah.
- Masuk sebagai tamu tanpa akun.
- Data parameter dan tabel disimpan otomatis di localStorage browser; tersedia ekspor dan pemulihan backup JSON.
- Input foto dari galeri atau kamera.
- OCR memproses dua bagian foto secara terpisah, meningkatkan kontras, dan menggunakan rentang umum berat 10–20 g serta volume 0,5–2,9 mL sebagai petunjuk penyaringan.
- Hasil OCR tetap harus diverifikasi manual. OCR berbasis Tesseract.js tidak menjamin pembacaan tulisan tangan atau koma desimal secara benar.
- Foto hasil PNG memakai tata letak laporan yang lebih rapi.

## Rumus
FFA (%) = Volume titrasi (mL) × Normalitas NaOH × Faktor asam oleat ÷ Berat sampel (g)

Nilai awal: faktor 25.6; normalitas NaOH 0.0429.

## Penyimpanan
Data otomatis disimpan pada browser/perangkat yang sedang digunakan. Ini bukan sinkronisasi cloud dan bukan akun aman; hapus data browser atau ganti perangkat dapat menghilangkan data. Unduh backup JSON secara berkala dan simpan terpisah. Jangan memasukkan data rahasia ke perangkat bersama.

## GitHub Pages
Unggah seluruh isi ZIP ke root repository, termasuk `.github/workflows/deploy.yml`, lalu pastikan Settings → Pages menggunakan GitHub Actions.
