
---

### 📄 `handbook/02-gitignore.md`


# 02 – `.gitignore`: Penjaga Gerbang ke GitHub

`.gitignore` adalah file yang berisi daftar **file/folder yang tidak boleh ikut ter-commit** ke Git.

Ini penting banget buat vibe coder karena:
- Banyak yang commit `.env`
- Banyak yang commit `node_modules`
- Repo jadi berat dan bocor sekaligus 😅


 ✍️ Contoh `.gitignore` minimal untuk fullstack

```gitignore
# Env
.env
.env.*

# Dependency
node_modules/

# Build output
dist/
build/
.next/

# OS & editor
.DS_Store
.vscode/
.idea/
```

---

Kalau mau versi lebih lengkap, lihat:

```bash
templates/.gitignore-universal
```

## 🧠 Mindset yang benar

Sebelum commit:

Cek: git status

Pastikan tidak ada:

- **.env**

- File yang berisi password / key
---

### Kalau terlanjur kebawa:

1. Tambah ke .gitignore

2. Hapus dari staging: git reset HEAD nama-file

3. Rotate credential jika sudah ter-push ke remote

---

## 💡 Tips untuk vibe coder

Saat buat project baru inisialisasi Git dengan cara:
```bash
git init
```

Kemudian buat .gitignore dulu, baru mulai minta AI generate kode

Ini kebiasaan kecil, tapi efeknya besar.