# IoT Smart Farming

## Deskripsi Proyek
IoT Smart Farming adalah proyek yang bertujuan untuk mengintegrasikan teknologi Internet of Things (IoT) dalam sektor pertanian. Proyek ini dirancang untuk membantu petani memantau kondisi tanah, kelembaban, dan suhu secara otomatis menggunakan sensor-sensor yang terhubung ke jaringan internet. Dengan sistem ini, petani dapat melakukan pemantauan jarak jauh dan membuat keputusan berbasis data untuk meningkatkan efisiensi pertanian.

## Fitur Utama
- **Pemantauan Kelembaban Tanah:** Mengukur kelembaban tanah menggunakan sensor yang secara real-time menampilkan data ke platform berbasis web.
- **Pengukuran Suhu Lingkungan:** Menggunakan sensor suhu untuk memantau kondisi iklim sekitar tanaman.
- **Notifikasi Otomatis:** Mengirimkan peringatan melalui aplikasi atau email jika kondisi tanah terlalu kering atau terlalu basah.
- **Pengendalian Sistem Irigasi:** Sistem irigasi otomatis yang dikendalikan berdasarkan data dari sensor kelembaban tanah, mengoptimalkan penggunaan air.
- **Akses Jarak Jauh:** Monitoring dan pengendalian dapat dilakukan dari jarak jauh menggunakan perangkat yang terhubung ke internet.

## Teknologi yang Digunakan
- **NodeMCU (ESP8266):** Mikrokontroler utama yang menghubungkan semua sensor ke internet.
- **Sensor Kelembaban Tanah:** Digunakan untuk mendeteksi tingkat kelembaban tanah.
- **DHT11 Sensor:** Mengukur suhu dan kelembaban lingkungan sekitar.
- **MQTT Protocol:** Digunakan untuk komunikasi antara perangkat dan server.
- **Blynk Application:** Aplikasi mobile yang memungkinkan pengguna memantau dan mengendalikan sistem dari jarak jauh.
- **Platform IoT Cloud:** Untuk menyimpan dan menampilkan data secara real-time.

## Cara Kerja
1. Sensor kelembaban tanah dan suhu lingkungan mengumpulkan data dari area pertanian.
2. NodeMCU memproses data tersebut dan mengirimkannya ke platform cloud IoT melalui protokol MQTT.
3. Data dapat dipantau oleh petani menggunakan aplikasi Blynk atau dashboard berbasis web.
4. Sistem irigasi akan menyala otomatis jika tanah terlalu kering, atau notifikasi dikirimkan jika kondisi tanah membutuhkan perhatian.
   
## Instalasi
Untuk menjalankan proyek ini, ikuti langkah-langkah berikut:
1. **Kloning repositori:**
    ```bash
    git clone https://github.com/Deshan555/IOT-Smart_Farming.git
    ```
2. **Instal pustaka yang diperlukan:**
   Pastikan kamu telah menginstal Arduino IDE, pustaka Blynk, dan pustaka MQTT di dalam Arduino IDE.  
3. **Unggah kode ke NodeMCU:**
   Sambungkan NodeMCU ke komputer dan unggah kode dari folder `src` ke perangkat.
4. **Konfigurasi Blynk:**
   - Buat akun Blynk dan buat proyek baru.
   - Dapatkan *auth token* dari proyek tersebut dan masukkan ke dalam kode.
5. **Jalankan sistem:**
   Hubungkan semua sensor ke NodeMCU dan mulai memantau dari aplikasi Blynk atau dashboard web.

## Cara Kontribusi
Kontribusi selalu diterima! Jika kamu menemukan masalah atau ingin meningkatkan proyek ini, silakan ajukan *pull request* atau buka *issue* di repositori ini.

1. *Fork* proyek ini.
2. Buat *branch* fitur baru: `git checkout -b feature-branch`.
3. Ajukan perubahan: `git commit -m 'Menambahkan fitur ini'`.
4. Kirim perubahan ke *branch* utama: `git push origin feature-branch`.
5. Buat *pull request*.
