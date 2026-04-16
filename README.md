# percetakan_online
Project Kelompok
1. Anisa Auliana Rizkika
2. Ibnu Sahrul Anwar 230202811
3. Ramzi Selpora Widiyanto

---
# 🖨️ Website Percetakan Online Berbasis IoT (ESP32)

## 📌 Deskripsi Project

Project ini adalah sistem **percetakan online berbasis website** yang terintegrasi dengan **mikrokontroler ESP32 (IoT)**.
User dapat melakukan pemesanan cetak secara online, dan sistem akan memproses serta memonitor status cetakan secara real-time.

---

# 🚀 Tahapan Pengembangan Sistem

## 🔷 1. Perencanaan Sistem

* Menentukan konsep:

  * Website percetakan online
  * Mitra percetakan
  * Integrasi IoT (ESP32)
* Menentukan fitur:

  * Login & register
  * Upload file
  * Pilih jenis cetak
  * Status order
  * **Admin management system**

---

## 🔷 2. Desain Sistem

* Arsitektur:

  * **Admin → User → Website → Database → ESP32 → Printer**
* Desain database:

  * Tabel `users`
  * Tabel `admin`
  * Tabel `mitra`
  * Tabel `orders`

---

## 🔷 3. Pembuatan Website (Frontend & Backend)

* Menggunakan:

  * HTML, CSS, Bootstrap
  * PHP (Native)
  * MySQL (Database)

### Fitur:

#### 👤 User:

* Login/register
* Upload file
* Order cetak
* Lihat status

#### 🛠️ Admin:

* Login admin
* Kelola user
* Kelola mitra percetakan
* Monitoring semua order
* Laporan data

#### Tambahan
* Halaman home
* Halaman Upload dan Custom Produk
* Halaman Pilih Percetakan (Maps)
* Halaman Cekout
* Halaman Tracking pesanan
* Dashboard Mitra Percetakan

---

## 🔷 4. Pembuatan REST API

* API untuk ESP32:

  * Ambil data order
  * Update status order
* Format data: JSON

---

## 🔷 5. Implementasi ESP32

* Koneksi WiFi
* Ambil data dari API
* Proses data (simulasi cetak)
* Update status ke server

---

## 🔷 6. Integrasi Sistem

Alur:

1. **Admin mengelola sistem (user & mitra)**
2. User melakukan order
3. Data masuk database
4. ESP32 mengambil data
5. Proses cetak
6. Update status
7. Website menampilkan status

---

## 🔷 7. Testing

* Uji login admin & user
* Uji upload file
* Uji koneksi database
* Uji API
* Uji komunikasi ESP32

---

## 🔷 8. Dokumentasi

* Flowchart sistem
* Diagram arsitektur
* Penjelasan:

  * ALU
  * Control Unit
  * Interrupt
  * Addressing Mode

---

# 📁 Struktur Folder Project

```
percetakan-iot/
│
├── 📁 frontend/                # Tampilan Website
│   ├── index.php
│   ├── login.php
│   ├── register.php
│   ├── dashboard.php
│   ├── upload.php
│   ├── admin/                 # Halaman Admin
│   │   ├── dashboard.php
│   │   ├── kelola_user.php
│   │   ├── kelola_mitra.php
│   │   └── laporan.php
│   └── assets/
│       ├── css/
│       ├── js/
│       └── images/
│
├── 📁 backend/                # Logic Server
│   ├── config/
│   │   └── koneksi.php
│   ├── models/
│   ├── controllers/
│   └── functions.php
│
├── 📁 api/                    # REST API untuk ESP32
│   ├── get_order.php
│   ├── update_status.php
│   └── koneksi.php
│
├── 📁 database/
│   └── percetakan.sql
│
├── 📁 esp32/                  # Kode Mikrokontroler
│   └── esp32.ino
│
├── 📁 docs/                   # Dokumentasi
│   ├── flowchart.png
│   ├── arsitektur.png
│   └── laporan.pdf
│
├── README.md
└── .gitignore
```

---

# 🔗 Alur Sistem

```
Admin → User → Website → Database → API → ESP32 → Printer
                          ↑                     ↓
                     Monitoring & Control ←-----
```

---

# 🛠️ Teknologi yang Digunakan

* Frontend: HTML, CSS, Bootstrap
* Backend: PHP Native
* Database: MySQL
* IoT: ESP32
* API: REST (JSON)

---

# 🎯 Tujuan Project

* Mempermudah pemesanan percetakan
* Mengintegrasikan sistem web dengan perangkat fisik
* Memberikan kontrol penuh kepada admin
* Menerapkan konsep IoT dalam dunia nyata

---

# 🔥 Pengembangan Selanjutnya

* Integrasi pembayaran online
* Notifikasi WhatsApp
* Tracking lokasi percetakan (Google Maps)
* Dashboard real-time

---

# 👨‍💻 Author

Nama: Ibnu SahrulAnwar
Project: Tugas Project Based Learning
