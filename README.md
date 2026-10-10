# Absensi Online X TKJ 1

## Fitur
- Logo sekolah di kiri dan logo X TKJ 1 di kanan.
- Nama, status Hadir/Sakit/Izin/Dispensasi/Alfa.
- Alasan diwajibkan untuk Sakit, Izin, Dispensasi, dan Alfa.
- Waktu hanya jam dan menit.
- Data disimpan dalam SQLite.
- Endpoint pemeriksaan: `/health`.

## Deploy ke Render
1. Upload `app.py`, `requirements.txt`, dan `render.yaml` ke repository GitHub.
2. Di Render pilih **New > Blueprint** lalu hubungkan repository.
3. Render membaca `render.yaml` dan membuat web service beserta persistent disk.
4. Setelah deploy selesai, buka URL `https://...onrender.com` yang ditampilkan Render.
5. Uji kirim absensi dari HP lain.

Catatan:
- Hosting publik membutuhkan akun dan proses deploy; file ini tidak bisa membuat URL publik sendiri hanya dengan menekan Run.
- Konfigurasi persistent disk di Render dapat menimbulkan biaya. Periksa harga dan ketentuan Render sebelum deploy.
- Terminal lokal HP tidak akan menerima log dari server hosting; log tersedia di dashboard layanan hosting.
- Jam server hosting mungkin menggunakan zona waktu UTC. Untuk waktu WIB, perlu pengaturan zona waktu atau konversi eksplisit.
