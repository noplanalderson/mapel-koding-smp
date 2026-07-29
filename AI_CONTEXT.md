# AI_CONTEXT.md

## Deskripsi Proyek

Proyek ini merupakan website pembelajaran interaktif mata pelajaran Koding dan KA SMP berdasarkan Kurikulum Merdeka.

Website dikembangkan sebagai media pembelajaran mandiri dan media ajar guru dengan fitur:

* Materi Interaktif
* Simulasi
* Game Edukasi
* Kuis
* Refleksi
* Sertifikat
* Integrasi Google Sheet
* Penyimpanan progres menggunakan Local Storage

Target pengguna:

* SMP Kelas 7
* SMP Kelas 8
* SMP Kelas 9

---

# Struktur Direktori
Di dalam direktori kelas, untuk setiap file materi gunakan prefix 1-* atau 2-* sesuai dengan semesternya.

```text
/
│
├── index.html
│
├── 7/
│   ├── index.html
│   ├── 1-materi-1.html
│   ├── 2-materi-2.html
│   └── 2-materi-n.html
│
├── 8/
│   ├── index.html
│   ├── 1-materi-1.html
│   ├── 1-materi-2.html
│   └── 2-materi-n.html
│
├── 9/
│   ├── index.html
│   ├── 1-materi-1.html
│   ├── 2-materi-2.html
│   └── 2-materi-n.html
│
└── assets/
    ├── css/
    ├── js/
    ├── images/
    ├── icons/
    └── audio/
```

---

# Halaman Utama

## index.html

Menampilkan:

* Logo Website
* Judul Portal Pembelajaran Koding dan KA SMP
* Pilihan Kelas:

  * Kelas 7
  * Kelas 8
  * Kelas 9
* Progress Pembelajaran
* Statistik Materi Selesai
* Badge yang diperoleh siswa

---

# Standar Halaman Materi

Setiap materi WAJIB memiliki menu berikut:

1. Beranda
2. Tujuan Pembelajaran
3. Materi
4. Simulasi
5. Game Interaktif
6. Kuis
7. Refleksi
8. Sertifikat

---

# Standar UI/UX

## Tema

* Modern
* Edukatif
* Ramah siswa SMP
* Mobile First
* Responsif

## Warna

Kelas 7:

* Biru
* Hijau

Kelas 8:

* Ungu
* Biru

Kelas 9:

* Biru
* Cyan

## Efek

Gunakan:

* Transisi halus
* Progress bar
* Confetti saat lulus
* Badge Achievement
* Animasi ringan

Hindari:

* Animasi berlebihan
* Pop-up mengganggu
* Loading yang lambat

---

# Standar Materi

Materi harus:

* Menggunakan bahasa sederhana
* Mudah dipahami siswa SMP
* Mengandung ilustrasi visual
* Mengandung contoh kehidupan sehari-hari
* Mengandung aktivitas interaktif

Setiap sub materi minimal memiliki:

* Penjelasan
* Contoh
* Aktivitas interaktif

---

# Standar Simulasi

Simulasi harus:

* Berbasis browser
* Tidak membutuhkan server
* Memberikan feedback langsung
* Menampilkan hasil secara visual

Contoh:

* Drag and Drop
* Matching
* Interactive Diagram
* Sandbox sederhana

---

# Standar Game

Game harus:

* Edukatif
* Mendukung tujuan pembelajaran
* Memiliki skor
* Memiliki level
* Memiliki reward

Elemen wajib:

* Score
* Timer (opsional)
* Progress
* Feedback benar/salah

---

# Standar Kuis

Sebelum kuis dimulai:

Siswa wajib mengisi identitas.

## Form Identitas

Nama Siswa:

* Text Input
* Required

Kelas:

* Dropdown
* Required

Pilihan:

* Kelas 7A
* Kelas 7B
* Kelas 8A
* Kelas 8B
* Kelas 9A
* Kelas 9B

Validasi:

* Nama tidak boleh kosong
* Kelas wajib dipilih

Tombol "Mulai Kuis" hanya aktif jika seluruh data valid.

---

## Kuis

Ketentuan:

* 10 soal pilihan ganda
* Satu soal per halaman
* Tombol Next
* Tombol Previous
* Penilaian otomatis

Kategori nilai:

90–100:
Sangat Baik

80–89:
Baik

70–79:
Cukup

<70:
Perlu Belajar Lagi

---

## Penyimpanan Data

Data yang disimpan:

* Nama
* Kelas
* Nilai
* Jumlah Benar
* Jumlah Salah
* Persentase
* Tanggal
* Waktu

Simpan ke:

* Canva Sheet
* Local Storage

---

# Sertifikat

Jika nilai >= 70

Tampilkan:

* Nama siswa
* Kelas
* Nama materi
* Nilai
* Tanggal

Sediakan tombol:

* Download PNG
* Download PDF

Jika nilai < 70

Tampilkan pesan:

"Silakan pelajari kembali materi dan coba kuis lagi."

---

# Refleksi

Minimal berisi:

1. Apa yang saya pelajari hari ini?
2. Materi apa yang paling saya pahami?
3. Materi apa yang masih sulit?
4. Bagaimana saya menerapkannya dalam kehidupan sehari-hari?

Jawaban disimpan ke Local Storage.

---

# Teknologi

Gunakan:

* HTML5
* CSS3
* Vanilla JavaScript

Hindari:

* Framework berat
* Backend server
* Dependensi eksternal yang tidak diperlukan

---

# Template Prompt AI Agent

Ketika membuat materi baru, gunakan template berikut.

---

Buatkan multimedia pembelajaran interaktif mata pelajaran Koding dan KA SMP berdasarkan standar pada AI_CONTEXT.md.

Informasi Materi:

Kelas:
[NAMA KELAS]

Materi:
[NAMA MATERI]

Tujuan Pembelajaran:
[TUJUAN PEMBELAJARAN]

Sub Materi:

1. [SUB MATERI 1]
2. [SUB MATERI 2]
3. [SUB MATERI 3]
4. [SUB MATERI N]

Ketentuan:

* Ikuti seluruh standar pada AI_CONTEXT.md.
* Buat halaman Beranda, Materi, Simulasi, Game, Kuis, Refleksi, dan Sertifikat.
* Buat 10 soal kuis pilihan ganda.
* Tambahkan game edukatif yang relevan dengan materi.
* Tambahkan simulasi interaktif yang relevan dengan materi.
* Gunakan Local Storage untuk progres belajar.
* Integrasikan hasil kuis dengan Google Sheet.
* Gunakan desain modern dan responsif.
* Seluruh fitur harus berjalan langsung di browser tanpa backend.

Output yang dihasilkan harus berupa file html yang sudah lengkap dan siap digunakan.

```
```
