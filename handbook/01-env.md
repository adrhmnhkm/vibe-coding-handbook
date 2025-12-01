# 01 – Apa itu `.env` dan kenapa penting?

Di dunia vibe coding, masalah paling sering terjadi adalah:
- API key di-hardcode di kode
- Password database ada di `index.js`
- Token SMTP nongol di GitHub

Semua ini **seharusnya** disimpan di file terpisah bernama `.env`.

---

## 🔐 Fungsi `.env`

File `.env` digunakan untuk menyimpan:

- API key (Stripe, Midtrans, Firebase, dll.)
- URL database + username + password
- Token email (SMTP, Brevo, Mailgun)
- Secret untuk JWT

Contoh:

```bash
DATABASE_URL=postgres://user:pass@localhost:5432/dbname
JWT_SECRET=super-rahasia
SMTP_USER=akun@domain.com
SMTP_PASS=password-sangat-rahasia
```

---

## ⚠️ Aturan .env

Jangan pernah commit .env ke GitHub

.env hanya hidup di:

- Laptop / PC kamu

- Server / VPS

- Secret manager platform (Vercel, Netlify, dsb.)

### Di repo publik:

- Yang boleh: .env.example

- Yang tidak boleh: .env asli

---

🧩 Cara pakai .env di Node.js (Express)

Install dependency:

npm install dotenv


Lalu di app.js atau index.js:

import "dotenv/config";

const port = process.env.PORT || 3001;
const dbUrl = process.env.DATABASE_URL;


Di backend, selalu ambil nilai dari process.env, bukan string langsung.

✅ Pola sehat untuk vibe coder

Saat minta AI generate backend, biasakan tulis di prompt:

“Jangan hardcode credential apa pun, semua konfigurasi (database URL, JWT secret, SMTP, dsb.) harus diambil dari environment variables.”

Dengan begitu, AI akan otomatis menyusun kode yang menggunakan process.env daripada string literal.

Kalau sudah paham ini, vibe coding kamu naik satu level. 🚀
