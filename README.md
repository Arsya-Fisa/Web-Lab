# Web Lab & Manajemen Sarpras Kampus

Sistem informasi berbasis web yang dirancang untuk mengelola peminjaman laboratorium dan fasilitas sarana prasarana (sarpras) di lingkungan kampus.

---

## 👥 Peran & Kontribusi Tim
* **Arsya Fikri Sabilillah**: Systems Analyst & Database Evaluator
  * **Tanggung Jawab Utama**:
    1. Memetakan alur kelola layanan dan kategori sarpras menggunakan Activity Diagram.
    2. Merancang validasi alur input form agar sistem memvalidasi data di tingkat aplikasi sebelum diproses ke basis data.
    3. Merapikan struktur basis data relasional serta melakukan *data cleaning* data sarpras menggunakan Microsoft Excel.
    4. Melakukan pengujian fungsional (*Blackbox Testing*) pada form input data sarpras.

---

## 📐 Dokumentasi Analisis Sistem (Activity Diagram)
Berikut adalah pemetaan alur fungsional kelola layanan sarpras yang saya evaluasi:

* **Alur Kelola Layanan (Admin - System - Database)**:
  * Pemisahan alur validasi input: Jika format data tidak valid, sistem langsung memunculkan notifikasi gagal tanpa mengirim *query* kosong ke basis data.

---

## 🧪 Dokumentasi Pengujian & Validasi Data (QA & SQL)
Contoh skenario pengujian fungsional dan validasi data yang saya lakukan:

| Fitur / Alur | Skenario Pengujian | Hasil yang Diharapkan | Status |
| :--- | :--- | :--- | :--- |
| **Input Layanan** | Admin menambah layanan baru dengan form lengkap | Data tersimpan di basis data & muncul notifikasi sukses | PASS |
| **Validation Check**| Admin mengirim form dengan kolom wajib yang kosong | Sistem menolak proses simpan & memunculkan pesan peringatan | PASS |
| **Hapus Layanan** | Admin menghapus data kategori sarpras | Sistem memproses penghapusan & memperbarui data relasional | PASS |
