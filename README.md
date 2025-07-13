# WordPress BruteForcer

![Build Status](https://img.shields.io/badge/build-passing-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)
![Python](https://img.shields.io/badge/python-3.x-blue.svg)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20macOS%20%7C%20Termux-lightgrey)
![Stars](https://img.shields.io/github/stars/LikeEx01/WpBruteforce?style=social)
![Issues](https://img.shields.io/github/issues/LikeEx01/WpBruteforce)
![Last Update](https://img.shields.io/github/last-commit/LikeEx01/WpBruteforce)

---

![Preview](https://f.top4top.io/p_3480sg1tk4.jpg)

---

## Deskripsi

**XML-RPC WordPress BruteForcer** adalah tool Python otomatis untuk mengeksploitasi endpoint `xmlrpc.php` WordPress melalui metode `wp.getUsersBlogs`, yang memungkinkan bruteforce login dengan kombinasi username dan password umum. Tool ini mengekstrak username secara otomatis dari REST API endpoint `/?rest_route=/wp/v2/users` dan memverifikasi langsung ke halaman `/wp-login.php` dan `/wp-admin`.

---

## Fitur Utama

- 🔍 **Auto Extract Username** dari `/?rest_route=/wp/v2/users`
- 🔐 **BruteForce** via XML-RPC (`xmlrpc.php`) menggunakan metode `wp.getUsersBlogs`
- ✅ **Validasi Otomatis** ke `/wp-login.php` dan `/wp-admin/`
- 📝 **Logging Otomatis** ke file `RidSucess.txt` dan `RidFailed.txt`
- 🚀 **Support Multithreading** (default 10 thread)
- 🌈 **Output Berwarna ANSI** untuk terminal yang mendukung warna
- 🌐 **Compatible** dengan semua OS: Termux, Linux, Windows, Arch, WSL

---

## Persyaratan

- Python 3.x
- Library Python:
  - `requests`
  - `urllib3`

---

## Instalasi

### 📱 Termux / Android
```bash
pkg update -y
pkg install git python -y
pip install requests urllib3
git clone https://github.com/LikeEx01/WpBruteforce.git
cd WpBruteforce
python3 WpBruteforce.py
```

### 💻 Windows (CMD / PowerShell)
1. Install Python: https://www.python.org/downloads/
2. Jalankan:
```bash
pip install requests urllib3
git clone https://github.com/LikeEx01/WpBruteforce.git
cd WpBruteforce
python WpBruteforce.py
```

### 🐧 Linux / Ubuntu / Debian
```bash
sudo apt update && sudo apt install git python3 python3-pip -y
pip3 install requests urllib3
git clone https://github.com/LikeEx01/WpBruteforce.git
cd WpBruteforce
python3 WpBruteforce.py
```

### 🐧 Arch Linux / Manjaro
```bash
sudo pacman -Sy git python --noconfirm
pip install requests urllib3
git clone https://github.com/LikeEx01/WpBruteforce.git
cd WpBruteforce
python3 WpBruteforce.py
```

---

## Penggunaan

1. Buat file berisi daftar target, misalnya `list.txt`:
```
http://example.com
https://target-site.id
targetdomain.org
```

2. Jalankan script:
```bash
python3 WpBruteforce.py
```

3. Saat diminta:
```
MASUKAN FILE LISTE SITE: list.txt
```

4. Tool akan otomatis mencari username dari REST API, lalu melakukan bruteforce, dan mencetak hasil secara real-time.

---

## Output

- ✅ **`RidSucess.txt`**
  > Daftar login yang berhasil  
  Format:  
  ```
  http://target.com/wp-login.php#admin@admin123
  ```

- ❌ **`RidFailed.txt`**
  > Daftar user yang gagal login  
  Format:  
  ```
  http://target.com/wp-login.php#admin
  ```

---

### Contoh Output di Terminal
```bash
[ INFO ] http://targetsite.com - Berhasil !!
USER: admin PASS: admin123

[ INFO ] http://targetsite.com - Gagal !!
USER: admin PASS: password123
```

---

## Penafian

> ⚠️ **PERINGATAN:**  
Tool ini hanya untuk tujuan edukasi dan pengujian keamanan pada sistem milik sendiri atau yang telah diberikan izin tertulis.  
Segala penyalahgunaan terhadap sistem orang lain adalah **ilegal** dan sepenuhnya menjadi tanggung jawab pengguna.  
Developer tidak bertanggung jawab atas segala bentuk penyalahgunaan.

---

## Lisensi

Tool ini dirilis di bawah [MIT License](https://opensource.org/licenses/MIT)

---

## Kontak

- GitHub: [LikeEx01](https://github.com/LikeEx01)
- Telegram: [LikeEx01](https://t.me/usernamee1337)

---

## 🔔 Bergabung di Saluran WhatsApp

Untuk update, pengumuman, dan informasi lainnya, silakan bergabung di saluran WhatsApp resmi kami:

👉 [https://whatsapp.com/channel/0029VaudLHc7YSd9S9c9800c](https://whatsapp.com/channel/0029VaudLHc7YSd9S9c9800c)

---

**Terima kasih telah menggunakan WordPress XML-RPC BruteForcer by LikeEx01 ❤️**
