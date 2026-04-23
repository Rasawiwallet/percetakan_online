# IoT System Parking
Project Kelompok
1. Anisa Auliana Rizkika ()
2. Ibnu Sahrul Anwar 230202811 ()
3. Ramzi Selpora Widiyanto ()
4. Ali Jati Utomo ()

---

🧠 1. Konsep Sistem Smart Parking IoT
Sistem terdiri dari 3 bagian utama:
1. Gate masuk (ambil karcis)
2. Area parkir (deteksi slot kosong)
3. Gate keluar (validasi karcis + buka palang)

⚙️ 2. Struktur Alat (Hardware)
A. Mikrokontroler Utama
-ESP32 DevKit V1
Fungsi:
--Otak sistem
--Koneksi WiFi (IoT)
--Kirim data ke web/app

B. Sistem Gate Masuk (IN)

![contoh hasil](gambar/contoh_gambaran.jpg)

Komponen:
-Sensor kendaraan: Ultrasonic / IR
-Push button (ambil tiket)
-Thermal printer mini / LCD (opsional)
-Servo motor (palang)
-Buzzer

Fungsi:
-Deteksi kendaraan datang
-User tekan tombol → cetak / generate karcis
-Palang terbuka otomatis

C. Sistem Area Parkir

![contoh hasil](gambar/contoh_gambaran1.jpg)

Komponen:
-Sensor tiap slot:
-Ultrasonic / IR
-LED indikator:
-Hijau = kosong
-Merah = terisi

Fungsi:
-Deteksi ketersediaan parkir
-Kirim data ke ESP32 → tampil di web

D. Sistem Gate Keluar (OUT)

[gambar](gambar/contoh_gambar3.jpg)
[gambar](gambar/contoh_gambar4.jpg)

Komponen:
-RFID reader / barcode scanner
-Servo motor (palang keluar)
-LCD display (info pembayaran)
-Buzzer

Fungsi:
-Scan karcis
-Hitung durasi parkir
-Validasi → palang terbuka
