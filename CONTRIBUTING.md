# Panduan Kontribusi

Terima kasih sudah tertarik berkontribusi ke **Vibe Coding Handbook** 🙌  
Proyek ini dirancang agar **pemula pun bisa ikut kontribusi**.

---

## 👣 Bentuk Kontribusi yang Diterima

Kamu bisa berkontribusi dalam bentuk:

- Menambahkan bab baru di `handbook/`
- Menambahkan contoh kode atau template di `templates/`
- Menambahkan panduan framework di `guides/`
- Memperbaiki typo, kalimat membingungkan, atau struktur penjelasan
- Menambahkan referensi tools (secret scanner, linter, dsb.)
- Menerjemahkan konten ke bahasa lain (nanti kalau sudah siap)

---

## 🗂 Struktur Folder

- `handbook/` → penjelasan konsep & best practice
- `templates/` → contoh konkret (.env, .gitignore, docker-compose, dsb.)
- `guides/` → panduan alur / tutorial berbasis studi kasus

Jika menambah file baru, gunakan nama file yang deskriptif, misalnya:
- `08-logging-dan-monitoring.md`
- `vibe-nextjs.md`, dll.

---

## 🧱 Langkah Kontribusi Teknis

1. **Fork** repo ini ke akun GitHub kamu
2. **Clone** ke lokal:
   ```bash
   git clone https://github.com/USERNAME/vibe-coding-handbook.git
   cd vibe-coding-handbook
3. **Buat branch baru:**
   ```bash
   git checkout -b feature/nama-fitur

4. **Lakukan perubahan (tambah file, edit, dsb.)**

5. **Cek ulang:**

   - Tidak ada file sensitif (tidak ada .env asli, key, password, dsb.)
   - Konten mengikuti gaya bahasa santai tapi sopan

6. **Commit:**
   ```bash
   git add .
   git commit -m "Tambah panduan X"  # jelaskan singkat

7. **Push ke fork kamu:**
   ```bash
   git push origin feature/nama-fitur

8. **Buat Pull Request (PR) ke branch main di repo ini.**

---

## ✍️ Gaya Penulisan

Bahasa: Indonesia dulu (boleh campur istilah teknis Inggris)

Gunakan Markdown:

# untuk judul utama

## untuk subjudul

Gunakan list / tabel jika membuat langkah-langkah

### Contoh:

## Apa itu .env?

File `.env` digunakan untuk menyimpan konfigurasi rahasia seperti:

- API key
- Password database
- Token SMTP

## ⚠️ Hal yang Tidak Diperbolehkan

- Menyisipkan kredensial asli (API key, password, token, dsb.)
- Copy-paste konten berhak cipta secara mentah dari buku / blog / kursus
- Menyerang / merendahkan orang atau komunitas tertentu

- Menyertakan kode berbahaya tanpa konteks edukasi yang jelas

## 💬 Butuh Bantuan?

- Kalau bingung mau mulai kontribusi dari mana, kamu bisa:

- Lihat daftar issue dengan label good first issue

- Buka issue baru untuk tanya ide / minta arahan

- Terima kasih sudah membantu menjadikan internet tempat belajar ngoding yang lebih aman dan sehat. 🙏
