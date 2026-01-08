# Claude Coding Guidelines - Edu Project

## 1. Tech Stack & Constraints
- **Core:** Pure HTML5, Tailwind CSS, Alpine.js.
- **Dependencies:** Usahakan *zero-dependency*. Jika butuh icon, gunakan SVG inline.
- **Assets:** Script dan Style sebaiknya *internal* (di dalam file HTML) untuk file materi agar file bersifat *portable* (single-file distribution), kecuali ada `style.css` global di root.

## 2. Naming Conventions
- **Folder Jenjang:** `paud`, `tk-a`, `tk-b`, `sd-[1-6]`, `smp-[1-3]`, `sma-[1-3]`, `smk-[kejuruan]-[1-4]`.
- **Folder Mapel:** *kebab-case* (contoh: `matematika`, `sains`, `bahasa-indonesia`, `sosial`, `islam`, `english`, `fisika`, `kimia`, `biologi`, `olahraga`, `musik`, `seni-rupa`, `kewarganegaraan`, `ekonomi`, `geografi`).
- **Folder Topik:** `[nomor_urut]-[topik]`
  - Topik harus granular sesuai kurikulum pada jenjang. Tidak terlalu luas, tidak terlalu spesifik.
  - Contoh: `001-hukum-newton`
- **File:** `[tipe].html`
  - Contoh: `teori.html`, `latihan.html`, `evaluasi.html`, `rangkuman.html`.

## 3. Code Structure (Boilerplate)
Setiap file HTML harus memiliki struktur dasar berikut:
- Meta viewport untuk responsivitas mobile.
- Navigasi sederhana pada index.html menggunakan iframe (Back to Home, Next/Prev Lesson).
- Footer dengan copyright.
- **Color Palette:**
  - PAUD/TK/SD: Warna cerah, playful, font besar/bulat (misal: Comic Neue atau Sans-Serif rounded).
  - SMP/SMA: Warna bersih, modern, minimalis, font profesional (Sans-Serif).

## 4. Content Guidelines per Tipe File

### A. Teori (`teori.html`)
- Fokus pada *readability*.
- Gunakan tag semantik (`<article>`, `<section>`, `<figure>`).
- Sertakan tombol "Lanjut ke Latihan" di bagian bawah.

### B. Latihan (`latihan.html`)
- **Interaktivitas:** Wajib ada. Contoh: Drag & Drop, Pilihan Ganda, Isian Singkat.
- **Feedback:** Immediate feedback. Jika user salah, beri tahu kenapa salah. Jika benar, beri animasi/pujian.
- Tidak ada scoring permanen, tujuannya *drill* pemahaman.

### C. Evaluasi (`evaluasi.html`)
- Format seperti kuis/ujian.
- **Feedback:** Delayed. Hasil skor dan kunci jawaban baru muncul setelah tombol "Submit" ditekan.
- Gunakan LocalStorage (opsional) untuk menyimpan progress sederhana.

### D. Rangkuman (`rangkuman.html`)
- Format seperti rangkuman materi.
- Recall teori dan latihan.
- Bahas flashback dan flashforward untuk menghubungkan ke materi lainnya.

## 5. Accessibility (A11y)
- Semua `<img>` wajib memiliki `alt` text yang deskriptif (penting untuk edukasi).
- Kontras warna harus memenuhi standar WCAG AA.
- Form input harus memiliki `<label>`.

## 6. Tone of Voice (Isi Materi)
- **PAUD - SD Kelas 3:** Menggunakan kata sapaan "Adik-adik", bahasa ceria, kalimat pendek.
- **SD Kelas 4 - SMP:** Sapaan "Teman-teman", bahasa kasual tapi edukatif.
- **SMA:** Sapaan "Rekan-rekan" atau netral, bahasa formal akademis namun mudah dipahami.