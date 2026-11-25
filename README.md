# Calculator Smart Scanner V5

Aplikasi web/PWA statis untuk perhitungan laboratorium.

## Modul aktif
- FFA: Volume × Normalitas NaOH × Faktor FFA ÷ Berat sampel.
- Kadar Air: (Berat botol kosong + berat sampel − berat akhir) ÷ berat sampel × 100%.
- AV: 56,1 × Normalitas KOH × volume titrasi ÷ (berat labu akhir − berat labu kosong).
- FC: (Berat akhir − berat awal) ÷ berat sampel × 100%.
- Kadar Abu: (Berat akhir − berat awal) ÷ berat sampel × 100%.

POV ditampilkan sebagai fitur dalam pengembangan.

## Fitur
Riwayat terpisah per kalkulator, penyimpanan otomatis di browser, pengaturan normalitas dan presisi desimal, baris dinamis, baris kosong/tidak lengkap dilewati, backup dan pemulihan JSON. FFA memiliki OCR bantuan dan ekspor foto sederhana.

## Deploy GitHub Pages
1. Unggah isi ZIP ke branch `main`.
2. Pastikan workflow `.github/workflows/deploy.yml` ikut terunggah.
3. Settings > Pages > Source: GitHub Actions.
4. Tunggu workflow selesai.

## Catatan
Penyimpanan otomatis berada di browser/perangkat yang digunakan, bukan cloud. Unduh backup secara berkala. OCR dapat keliru, terutama untuk tulisan tangan; verifikasi angka sebelum dipakai. Hasil kalkulasi perlu diverifikasi dengan metode dan SOP laboratorium.
