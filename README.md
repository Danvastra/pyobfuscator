# 🔐 pyobfuscator v1.0

**pyobfuscator v1.0** adalah tools Python sederhana untuk **menyamarkan (obfuscate) file `.py`** agar source code asli **tidak mudah dibaca**, namun **program tetap bisa dijalankan normal** oleh user.

Project ini dibuat untuk **edukasi, showcase GitHub**, dan perlindungan ringan terhadap **copy–paste source code**.

> ⚠️ Catatan: Ini adalah **obfuscation**, bukan enkripsi kriptografi tingkat tinggi.

---

## ✨ Fitur Utama

- 🔒 Obfuscate file Python secara otomatis
- ▶️ File hasil obfuscation **bisa langsung dijalankan**
- 🔑 De-obfuscation **wajib menggunakan KEY**
- ❌ Source code asli tidak terlihat di GitHub
- 📦 Tidak memerlukan library tambahan (pure Python)
- 🧭 Menu CLI yang sederhana & rapi

---

## 🧠 Konsep Kerja

### 🔐 Samarkan File
- User **membuat KEY / PASSWORD**
- Source code:
  - Di-XOR menggunakan key
  - Di-encode menggunakan Base64
- Key **tidak ditampilkan sebagai string polos**
- File hasil:
  - Aman untuk di-upload ke GitHub
  - Bisa dijalankan tanpa input key

### ▶️ Jalankan File Obfuscated
- User **tidak perlu memasukkan key**
- Program berjalan normal seperti biasa
- Source code asli tetap tersembunyi

### 🔓 Pudarkan (De-obfuscate)
- **Hanya pemilik file** yang bisa mengembalikan source
- Wajib memasukkan KEY yang benar
- Salah / tanpa key → gagal

---

## 📋 Menu Program
- Samarkan file (buat key)
- Pudarkan file (butuh key)
- Keluar

