
# Geetak - Kontrol USB Relay dengan CLI !

![PyPI](https://img.shields.io/pypi/v/geetak) ![License](https://img.shields.io/github/license/muflihnurfaizi/geetak) ![Python](https://img.shields.io/badge/python-3.8%2B-blue)

**Geetak** adalah aplikasi berbasis CLI (Command-Line Interface) untuk mengontrol USB relay secara efisien. Aplikasi ini memanfaatkan protokol HID untuk menghubungkan perangkat USB relay dengan komputer Anda. Dengan **Geetak**, Anda dapat mengatur timer, memeriksa perangkat, dan menyinkronkan waktu dengan server NTP secara langsung melalui terminal.

---

## ✨ Fitur Utama
- **Kontrol Timer**: Mengaktifkan relay pada waktu tertentu.
- **Sinkronisasi Waktu**: Menyinkronkan waktu lokal dengan server NTP.
- **Cek Perangkat**: Memastikan perangkat USB relay Anda tersedia.
- **Zona Waktu**: Menyesuaikan zona waktu untuk waktu lokal.
- **Progress Bar**: Menampilkan progres timer dengan tampilan interaktif.

---

## 🚀 Instalasi

### 1. Persyaratan
Pastikan Anda sudah menginstal Python versi **3.8 atau lebih baru**.

### 2. Instalasi dengan `pip`
Jalankan perintah berikut untuk menginstal Geetak:
```bash
pip install geetak
```

### 3. Verifikasi Instalasi
Setelah instalasi selesai, pastikan Geetak terinstal dengan benar:
```bash
geetak --help
```

Jika berhasil, Anda akan melihat daftar perintah yang tersedia.

---

## 🛠️ Cara Penggunaan

### 1. Memulai Timer
Gunakan perintah `gas` untuk mengatur timer dan mengaktifkan relay pada waktu tertentu:
```bash
geetak gas 10:00:00 --offset 500
```

**Penjelasan**:
- `10:00:00`: Waktu target dalam format `HH:MM:SS`.
- `--offset`: Tambahan delay dalam milidetik (opsional).

### 2. Cek Waktu Server NTP
Gunakan perintah `cekwaktu` untuk menampilkan waktu lokal yang disinkronkan dengan server NTP:
```bash
geetak cekwaktu
```

### 3. Cek Perangkat
Gunakan perintah `cekalat` untuk memastikan perangkat USB relay tersedia:
```bash
geetak cekalat
```

### 4. Ubah Zona Waktu
Gunakan perintah `ubahzona` untuk menyesuaikan zona waktu (dalam jam):
```bash
geetak ubahzona +7
```

---

## 📖 Contoh Penggunaan
Berikut adalah contoh skenario penggunaan Geetak:

1. Anda ingin menghidupkan relay pada pukul **10:30:00 WIB** dengan tambahan delay **200 ms**:
   ```bash
   geetak gas 10:30:00 --offset 200
   ```

2. Anda ingin memeriksa apakah perangkat USB relay Anda sudah terhubung:
   ```bash
   geetak cekalat
   ```

3. Anda ingin menyinkronkan waktu lokal Anda dengan server NTP:
   ```bash
   geetak cekwaktu
   ```

---

## 💡 Tips dan Trik
- Pastikan perangkat USB relay Anda sudah terhubung sebelum menjalankan perintah.
- Gunakan perintah `ubahzona` untuk menyesuaikan zona waktu lokal Anda (misalnya, **+7** untuk WIB).

---

## 🛡️ Lisensi
Proyek ini dilisensikan di bawah lisensi [MIT](LICENSE).

---

## 🤝 Kontribusi
Kami terbuka untuk kontribusi! Jika Anda ingin membantu mengembangkan Geetak, silakan:
1. Fork repository ini.
2. Buat branch baru untuk fitur atau perbaikan Anda.
3. Kirimkan pull request.

---

## 📞 Dukungan
Jika Anda memiliki pertanyaan atau menemukan masalah, jangan ragu untuk menghubungi kami melalui [Issues](https://github.com/username/geetak/issues).

---

## ⭐ Dukung Kami
Jika Geetak bermanfaat untuk Anda, jangan lupa memberikan bintang ⭐ di repository ini!
