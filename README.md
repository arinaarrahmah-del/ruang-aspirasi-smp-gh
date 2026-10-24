# RUANG ASPIRASI SMP GALUH HANDAYANI

Starter website: GitHub Pages + Firebase Authentication + Cloud Firestore.

## Sebelum online
1. Buat proyek Firebase BARU bernama Ruang Aspirasi. Jangan gunakan Firebase Rutinan Semaan.
2. Tambahkan Web App di Project settings, lalu salin config web ke `index.html`, mengganti nilai `ISI_...`.
3. Authentication > Sign-in method: aktifkan Email/Password.
4. Buat Firestore Database.
5. Salin `firestore.rules` ke Firestore > Rules dan Publish.
6. Authentication > Users: buat akun admin, lalu salin UID.
7. Firestore: buat dokumen `admins/{UID}` dengan field `aktif` boolean `true`.
8. Masuk ke website sebagai admin, tambah semua 14 kegiatan lewat Kelola Kegiatan, lalu atur periode.

## GitHub Pages
Upload `index.html`, `firestore.rules`, `README.md` ke repository baru `ruang-aspirasi-smp-gh`. Lalu Settings > Pages > Deploy from a branch > `main` > `/(root)` > Save.

## Catatan
- Data lama Google Sheets dan proyek Rutinan Semaan tidak disentuh.
- Identitas responden diminta, jadi survei bukan anonim.
- Pertanyaan alasan manfaat selalu tampil, baik jawaban Ya maupun Tidak.
- Saran umum hanya satu kali di bagian akhir.
- Dashboard versi awal menyediakan ringkasan, filter kegiatan/kategori, dan ekspor CSV. PDF dan filter tahun/semester lanjutan dapat ditambahkan setelah alur dasar lolos uji.
- Uji dengan akun responden dan akun admin sebelum digunakan oleh seluruh sekolah.
