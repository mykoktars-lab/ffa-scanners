# Calculator Smart Scanner V6

Aplikasi web/PWA statis untuk perhitungan laboratorium.

## Modul aktif
- FFA: 25,6 × Normalitas KOH × volume titrasi ÷ berat sampel.
- Kadar Air: (berat botol kosong + berat sampel − berat akhir) ÷ berat sampel × 100%.
- AV: 56,1 × Normalitas KOH × volume titrasi ÷ (berat labu akhir − berat labu kosong).
- Kadar Abu: (berat akhir − berat awal) ÷ berat sampel × 100%.
- FC: (berat akhir − berat awal) ÷ berat sampel × 100%.

POV ditampilkan sebagai fitur dalam pengembangan.

## Fitur
Tampilan minimalis tanpa OCR/foto, pengaturan normalitas KOH bersama untuk FFA dan AV, faktor FFA 25,6 dan konstanta AV 56,1 ditetapkan di rumus, presisi desimal dapat diatur, input tersimpan otomatis pada perangkat, tombol Kosongkan Data tanpa riwayat, baris dinamis, serta baris kosong/tidak lengkap dilewati.

## Deploy GitHub Pages
1. Ekstrak ZIP dan unggah seluruh isi folder ke branch `main`.
2. Pastikan workflow `.github/workflows/deploy.yml` ikut terunggah.
3. Buka Settings > Pages dan pilih Source: GitHub Actions.
4. Tunggu workflow selesai.

## Catatan
Penyimpanan otomatis berada di browser/perangkat yang digunakan, bukan cloud. Hasil kalkulasi tetap perlu diverifikasi dengan metode dan SOP laboratorium.
