<h1 align="center">Vibe Coding Handbook</h1>

<p align="center">
  Build cepat. Deploy cepat. <br>
  Tapi gak ada lagi drama API key bocor di GitHub
</p>

<p align="center">
  <img src="https://img.shields.io/badge/license-MIT-green?logo=open-source-initiative&logoColor=white" />
  <img src="https://img.shields.io/badge/PRs-welcome-purple?logo=github&logoColor=white" />
  <img src="https://img.shields.io/badge/contributions-welcome-blue?logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/status-active-success?logo=rocket&logoColor=white" />
  <img src="https://img.shields.io/badge/made_for-beginner_coders-orange?logo=visualstudiocode&logoColor=white" />
</p>




> Panduan santai tapi serius untuk kamu yang suka ngoding pakai AI, biar tetap cepat **tanpa** bikin chaos, bocor kredensial, atau ngerusak server orang.

## 🎯 Tujuan 

Banyak orang sekarang bikin aplikasi pakai AI:
- ChatGPT, Gemini, Claude, dsb. nulis kodenya
- Developer tinggal _vibe_ ➝ copy paste ➝ deploy ➝ push ke GitHub

Masalahnya:
- API key sering di-hardcode
- `.env` ikut ke-commit
- Database bisa diakses publik
- Tagihan cloud bisa jebol karena mining / abuse

**Proyek ini ingin jadi:**
- Playbook / handbook berbahasa Indonesia
- Fokus ke **fullstack** (frontend + backend + deploy)
- Ditulis dengan gaya yang ramah buat pemula & vibe coder
- Tapi tetap mengikuti praktik keamanan dasar yang benar

---

## 📚 Isi Handbook

Semua materi utama ada di folder [`handbook/`](handbook):

1. `01-env.md` – Dasar `.env` dan kenapa ini penting
2. `02-gitignore.md` – Cara mencegah file sensitif ikut ke GitHub
3. `03-frontend-env.md` – Variabel environment di frontend (Next.js, React, dsb.)
4. `04-backend-security.md` – Praktik dasar keamanan backend
5. `05-auth-logic.md` – Login, session, JWT dengan cara yang bener
6. `06-ai-prompt-safe.md` – Contoh prompt aman saat minta AI nulis kode
7. `07-deploy-checklist.md` – Checklist sebelum deploy & push ke GitHub

Template ada di folder [`templates/`](templates):

- `.env.example` – Contoh struktur file env
- `.gitignore-universal` – Template `.gitignore` basic buat fullstack

Guides ada di folder [`guides/`](guides):

- `fullstack-vibe-coding.md` – Alur dari nol: bikin app fullstack pakai AI + best practice

---

## 👩‍💻 Untuk Siapa?

- Orang yang **baru belajar ngoding** tapi sudah pakai AI
- “Vibe coder” yang suka bikin projek iseng tapi mulai peduli kerapian
- Dev yang mau bantu edukasi adik-adik / junior soal keamanan basic
- Siapa pun yang mau bantu mengurangi kebocoran kredensial di GitHub 😀

---

## 🧩 Cara Menggunakan

1. Baca dulu file di `handbook/` sesuai kebutuhanmu
2. Pakai file di `templates/` sebagai contoh untuk projek kamu
3. Jika kamu pakai AI (ChatGPT, Gemini, dsb.), gunakan juga contoh prompt di:
   - `handbook/06-ai-prompt-safe.md`

---

## 🤝 Kontribusi

Kontribusi dari siapapun sangat diterima:

- Tambah bab baru di `handbook/`
- Tambah template `.env`, `.gitignore`, atau `docker-compose`
- Tambah panduan framework (Next.js, Laravel, Express, dsb.)
- Perbaiki penjelasan, typo, atau struktur

Silakan baca panduan lengkap kontribusi di:
- [`CONTRIBUTING.md`](CONTRIBUTING.md)

---

## 📜 Lisensi

Proyek ini menggunakan lisensi MIT. Silakan gunakan, modifikasi, dan bagikan selama tetap mencantumkan lisensi.

---

## ⭐ Dukung Proyek

Kalau kamu merasa terbantu:

- Kasih ⭐ ke repo ini di GitHub
- Share ke teman-teman yang suka vibe coding
- Pakai materi ini untuk ngajarin orang lain ngoding dengan lebih aman

Semoga bermanfaat dan bisa mengurangi drama “API key ke-push ke GitHub” di timeline kita semua. 😄
