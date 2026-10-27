# Campus Laboratory & Facility Management System

Sistem informasi berbasis web yang dirancang untuk mengelola peminjaman laboratorium, inventarisasi barang, dan fasilitas sarana prasarana (sarpras) di lingkungan kampus guna mengurangi pencatatan manual dan mencegah inkonsistensi data.

---

## 👥 Peran & Kontribusi Tim
* **Arsya Fikri Sabilillah**: Systems Analyst & Database Evaluator
  * **Tanggung Jawab Utama**:
    1. **Pemetaan Alur Sistem**: Memetakan alur fungsional seluruh modul (Sarpras, Layanan, dan Operasional Peminjaman) menggunakan Activity Diagram.
    2. **Perancangan Logika Validasi**: Merancang validasi input pada form aplikasi agar sistem dapat memfilter data invalid di tingkat antarmuka sebelum diproses ke basis data.
    3. **Evaluasi & Pengolahan Data**: Merancang skema relasi basis data (SQL) serta melakukan *data cleaning* data inventaris dan layanan menggunakan Microsoft Excel.
    4. **Quality Assurance (QA)**: Melakukan pengujian fungsional (*Blackbox Testing*) pada form penginputan data dan menjalankan kueri SQL dasar untuk memastikan tidak ada transaksi peminjaman yang 'gantung'.

---

## 📐 Dokumentasi Analisis Sistem (Activity Diagram)
Berikut adalah pemetaan alur fungsional kelola layanan dan validasi sistem yang saya evaluasi:

* **Alur Kelola Layanan (Admin - System - Database)**:
  * Pemisahan alur validasi input: Jika format data tidak valid, sistem langsung memunculkan notifikasi gagal di tingkat antarmuka tanpa mengirim *query* kosong yang membebani basis data.

---

## 🧪 Dokumentasi Pengujian & Validasi Data (QA & SQL)
Contoh skenario pengujian fungsional dan validasi data yang saya lakukan:

| Fitur / Alur | Skenario Pengujian | Hasil yang Diharapkan | Status |
| :--- | :--- | :--- | :--- |
| **Input Layanan** | Admin menambah layanan/barang baru dengan form lengkap | Data tersimpan di basis data & muncul notifikasi sukses | PASS |
| **Validation Check** | Admin mengirim form dengan kolom wajib yang kosong | Sistem menolak proses simpan & memunculkan pesan peringatan | PASS |
| **Data Integrity Check** | Menguji penghapusan data kategori/layanan terkait | Sistem memproses penghapusan & memperbarui relasi data secara akurat | PASS |
