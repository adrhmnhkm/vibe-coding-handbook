
---

### 📄 `handbook/03-frontend-env.md`


# 03 – Environment Variable di Frontend (Next.js / React)

Frontend modern (Next.js, React, Vite, dsb.) juga bisa pakai environment variable.

Tapi ada perbedaan penting:
- Di backend, `process.env` **tidak terlihat user**
- Di frontend, variabel tertentu akan dibundle dan bisa dilihat di browser

---

## 🔑 Next.js: `NEXT_PUBLIC_*`

Di Next.js:

- Variabel yang dimulai dengan `NEXT_PUBLIC_` ➝ dikirim ke browser
- Variabel tanpa prefix ➝ hanya tersedia di server (route handler / server component)

Contoh `.env.local`:

```bash
NEXT_PUBLIC_API_BASE_URL=https://api.example.com
JWT_SECRET=ini-harusnya-tidak-dikirim-ke-browser
```

### Di frontend:
```js
const apiUrl = process.env.NEXT_PUBLIC_API_BASE_URL;
```

Jangan pernah mengakses JWT_SECRET di komponen client.

### 💡 Apa yang aman di NEXT_PUBLIC_*?

Yang relatif aman:

- Base URL API
- Public key (misal: publik key payment)
- DSN Sentry atau sejenis (meski tetap harus hati-hati)
- Yang tidak aman:
- Secret key payment
- Password database
- Token admin
- JWT secret

---

## 🔐 Aturan main untuk vibe coder

Semua secret tetap di backend. Frontend hanya memegang:

1. Informasi non-rahasia

2. Token session yang memang didesain untuk client (misal: access token via cookie httpOnly)

Jika ragu, anggap saja:

“Kalau saya taruh di frontend, berarti seluruh dunia bisa lihat.”

Ini bikin keputusan lebih mudah.