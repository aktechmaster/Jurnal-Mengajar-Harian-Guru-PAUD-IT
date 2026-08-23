Berikut adalah draf dokumentasi **`README.md`** yang lengkap dan rapi untuk repositori proyek aplikasi **Jurnal Mengajar PAUD IT Al-Kautsar**:

---

# 📖 Jurnal Mengajar PAUD IT Al-Kautsar Mukomuko

Aplikasi Web **Jurnal Mengajar Harian** berbasis HTML, CSS, dan JavaScript Vanilla yang terintegrasi secara langsung dengan **Google Apps Script** dan **Google Sheets** sebagai *backend/database*.

Aplikasi ini dirancang untuk memudahkan para guru di PAUD IT Al-Kautsar dalam menginput laporan pembelajaran, pembiasaan ibadah, hafalan, pengamatan siswa, serta refleksi pengajaran harian secara digital, cepat, dan responsif melalui smartphone maupun komputer.

---

## ✨ Fitur Utama

* 🔄 **Dynamic Cascading Dropdowns (Filter Otomatis):**
* Mengambil data master guru, kelas, dan siswa secara *real-time* dari Google Sheets.
* Pilihan Nama Guru dan Kelas menyesuaikan secara otomatis berdasarkan **Unit** yang dipilih (Unit 1 / Unit 2).
* Pilihan Imam Shalat (Siswa) menyesuaikan secara otomatis berdasarkan **Kelas** yang dipilih.


* 💾 **Auto-Save Email Guru:** Menggunakan `localStorage` browser sehingga guru tidak perlu mengetik ulang alamat email setiap kali mengisi jurnal.
* 📊 **Integrasi Google Sheets Backend:** Data pengisian dikirimkan langsung ke basis data Google Sheets secara *asynchronous* (`fetch API`).
* 📱 **Desain Responsif & Ramah Pengguna:** Antarmuka visual yang disesuaikan dengan tema PAUD (warna lembut, kartu terpisah tiap bagian, font Nunito, dan layout grid yang responsif di layar ponsel).

---

## 📋 Struktur Form Jurnal Mengajar

Formulir terbagi ke dalam **4 Bagian Utama**:

| Bagian | Nama Bagian | Field / Input |
| --- | --- | --- |
| **Bagian A** | **Identitas Mengajar** | Email Guru, Unit, Nama Guru, Kelas, Pertemuan Ke-, Jumlah Siswa Hadir |
| **Bagian B** | **Pembiasaan & Hafalan** | Imam Shalat Dhuha, Imam Shalat Dzuhur, Hafalan Al-Qur'an, Hafalan Hadits, Hafalan Do'a |
| **Bagian C** | **Kegiatan Inti Pembelajaran** | Topik/Tema, Deskripsi Kegiatan, Media & Bahan Main / APE, Catatan Pengamatan Siswa |
| **Bagian D** | **Refleksi Guru** | Keberhasilan, Perbaikan, Rencana Tindak Lanjut (RTL) |

---

## 🛠️ Teknologi yang Digunakan

* **Frontend:** HTML5, CSS3 (*Custom CSS Variables, Flexbox, CSS Grid*), JavaScript (ES6+ Fetch API).
* **Typography & Assets:** [Google Fonts - Nunito](https://fonts.google.com/specimen/Nunito), Logo Unit (`logosit1.png`).
* **Backend / Database:** Google Apps Script (Web App Deployment) & Google Sheets.

---

## 🚀 Panduan Penggunaan & Peluncuran

### 1. Prasyarat (*Prerequisites*)

Pastikan file berikut berada dalam satu direktori/folder:

* `index.html` (Kode utama aplikasi)
* `logosit1.png` (Logo PAUD IT Al-Kautsar)

### 2. Menjalankan Aplikasi

1. Buka file `index.html` langsung menggunakan browser pilihan Anda (Chrome, Edge, Firefox, Safari) atau melalui server lokal (*Live Server* di VS Code).
2. Isi formulir secara berurutan mulai dari **Unit** untuk mengaktifkan filter otomatis nama guru dan kelas.
3. Klik tombol **Kirim Jurnal Mengajar** untuk menyimpan data ke Google Sheets.

### 3. Konfigurasi Backend (Google Apps Script)

URL *Web App* Google Apps Script dikonfigurasikan pada variabel `WEB_APP_URL` di dalam tag `<script>` pada file `index.html`:

```javascript
const WEB_APP_URL = "https://script.google.com/macros/s/AKfycbxDGnp8Zy1ojj40QyznCuVIp5UJboSGeWLHPDI7EfTWVFAb67cY3p3DEPF-9U_euifjhg/exec";

```

---

## 📄 Hak Cipta & Pengembang

```text
PAUD IT Al-Kautsar Mukomuko 2026 | Designed and Developed by aktechmaster

```
