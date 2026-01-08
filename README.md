# 📚 Pustaka Belajar Interaktif (Open Source)

Repository ini berisi kumpulan bahan ajar interaktif untuk berbagai jenjang pendidikan, mulai dari PAUD hingga SMA. Project ini dibangun menggunakan **Pure HTML, CSS, dan Vanilla JavaScript** agar ringan, mudah diakses, dan dapat dijalankan tanpa instalasi software yang kompleks.

Motivasi repo ini dibuat adalah memaksimalkan penggunaan Claude Code Max yang sudah di-subscribe bulanan, agar ter-utilisasi pada malam hari, saat tidak dipakai bekerja.

## 🗂 Struktur Kurikulum

Materi disusun berdasarkan jenjang pendidikan dan mata pelajaran:

* **Prasekolah:** `paud`, `tk-a`, `tk-b`
* **Sekolah Dasar:** `sd-1` s.d. `sd-6`
* **Sekolah Menengah Pertama:** `smp-1` s.d. `smp-3`
* **Sekolah Menengah Atas:** `sma-1` s.d. `sma-3`

## 📖 Format Materi

Setiap topik pembahasan dibagi menjadi 3 file terpisah untuk menjaga fokus belajar:

1.  **Teori (`*-teori.html`):** Penjelasan konsep, gambar ilustrasi, dan contoh kasus.
2.  **Latihan (`*-latihan.html`):** Soal interaktif dengan *feedback* langsung (benar/salah) untuk pemahaman.
3.  **Evaluasi (`*-evaluasi.html`):** Ujian pendek untuk mengukur penguasaan materi (skor muncul di akhir).
4.  **Rangkuman (`*-rangkuman.html`):** Rangkuman materi yang telah dipelajari.

## 🚀 Cara Menggunakan

### Untuk Siswa/Guru
1.  Download file `.zip` dari repository ini atau clone menggunakan Git.
2.  Buka folder jenjang yang diinginkan (misal: `sd-1/matematika`).
3.  Klik dua kali pada file `.html` untuk membukanya di browser (Chrome, Firefox, Edge, Safari).
4.  Tidak perlu koneksi internet (offline-ready) setelah file diunduh.

### Untuk Kontributor (Developer)
Kami menerima kontribusi modul baru! Pastikan Anda membaca `CLAUDE.md` atau guidelines kontribusi sebelum membuat Pull Request.

**Persyaratan Teknis:**
* HTML5 Semantik.
* Tailwind CSS Modern.
* Alpine JS.
* Responsive.

## 📄 Lisensi

Project ini dilisensikan di bawah [MIT License](LICENSE). Bebas digunakan untuk keperluan edukasi, sekolah, maupun belajar mandiri.

Pull Request sangat dihargai! Memang banyak yang kurang / salah / ngebug / tidak sesuai dengan kebutuhan, jadi silakan buat pull request-nya!