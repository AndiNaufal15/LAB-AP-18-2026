# LAB-AP-18-2026

## 📚 Repositori Tugas Praktikum Algoritma & Pemrograman 2026

Selamat datang di repositori resmi **Praktikum Algoritma & Pemrograman 2026**.

Repositori ini digunakan oleh mahasiswa untuk mengumpulkan seluruh **Tugas Praktikum (TP)** selama semester berlangsung melalui mekanisme **Fork** dan **Pull Request (PR)** di GitHub.

---

## 🛠️ Prasyarat (Requirements)

Sebelum memulai, pastikan Anda telah menyiapkan:

1. **Akun GitHub**
2. **Git CLI**
3. **Python**
4. **Text Editor / IDE** seperti Visual Studio Code atau PyCharm

Cek instalasi Git:

```bash
git --version
```

Cek instalasi Python:

```bash
python --version
```

atau:

```bash
python3 --version
```

---

## 📁 Struktur Repositori

Setiap mahasiswa memiliki folder khusus dengan format:

```text
<NIM> - <Nama Lengkap>
```

Contoh:

```text
LAB-AP-18-2026/
├── H071261041 - Aisyah Kamila/
│   ├── Praktikum-1/
│   │   ├── TP1_1_H071261041.py
│   │   └── TP1_2_H071261041.py
│   └── Praktikum-2/
│       └── TP2_1_H071261041.py
├── H071261042 - Abd. Faathir Ath Thaariq/
└── README.md
```

### Aturan Penamaan

| Elemen | Format | Contoh |
|---|---|---|
| Folder Mahasiswa | `<NIM> - <Nama Lengkap>` | `H071261041 - Aisyah Kamila` |
| Folder Praktikum | `Praktikum-<n>` | `Praktikum-1` |
| File Tugas | `TP<n>_<noSoal>_<NIM>.py` | `TP1_1_H071261041.py` |

---

# 🚀 Alur Pengumpulan Tugas

## 1. Fork Repository

Buka repository utama **LAB-AP-18-2026** di GitHub.

1. Klik **Fork**.
2. Pilih akun GitHub Anda.
3. Klik **Create fork**.

Setelah berhasil, Anda memiliki repository hasil fork pada akun GitHub sendiri.

```text
Repository utama:
OWNER/LAB-AP-18-2026

Repository fork:
USERNAME_ANDA/LAB-AP-18-2026
```

> **PENTING:** Kerjakan tugas pada repository hasil fork masing-masing.

---

## 2. Clone Repository Fork

Buka repository hasil fork, kemudian pilih:

```text
Code → HTTPS
```

Jalankan:

```bash
git clone https://github.com/USERNAME_ANDA/LAB-AP-18-2026.git
```

Kemudian:

```bash
cd LAB-AP-18-2026
```

---

## 3. Konfigurasi Identitas Git

Konfigurasi nama dan email Git:

```bash
git config user.name "USERNAME_GITHUB_ANDA"
git config user.email "EMAIL_GITHUB_ANDA"
```

Cek konfigurasi:

```bash
git config --list
```

---

## 4. Buat Branch Berdasarkan NIM

Setiap mahasiswa **WAJIB menggunakan branch berdasarkan NIM**.

Contoh:

```bash
git checkout -b H071261041
```

Cek branch:

```bash
git branch
```

Hasil:

```text
* H071261041
  main
```

> **Jangan mengerjakan tugas langsung pada branch `main`.**

---

## 5. Masuk ke Folder Mahasiswa

Masuk ke folder sesuai NIM dan nama:

```bash
cd "H071261041 - Aisyah Kamila"
```

---

## 6. Buat Folder Praktikum

Contoh untuk Praktikum 1:

```bash
mkdir Praktikum-1
cd Praktikum-1
```

Struktur:

```text
H071261041 - Aisyah Kamila/
└── Praktikum-1/
```

---

## 7. Simpan File Tugas

Gunakan format:

```text
TP<n>_<noSoal>_<NIM>.py
```

Contoh:

```text
Praktikum-1/
├── TP1_1_H071261041.py
├── TP1_2_H071261041.py
└── TP1_3_H071261041.py
```

---

## 8. Test Program

Pastikan program sudah berjalan dengan benar sebelum melakukan commit.

```bash
python TP1_1_H071261041.py
```

atau:

```bash
python3 TP1_1_H071261041.py
```

Pastikan:

- Program tidak menghasilkan error.
- Output sesuai dengan soal.
- Nama file sesuai ketentuan.
- Struktur folder sesuai ketentuan.

---

## 9. Cek Status

```bash
git status
```

---

## 10. Add File

Untuk menambahkan seluruh perubahan:

```bash
git add .
```

Atau satu file:

```bash
git add TP1_1_H071261041.py
```

Cek kembali:

```bash
git status
```

---

## 11. Commit

Contoh:

```bash
git commit -m "Menambahkan tugas Praktikum 1"
```

atau:

```bash
git commit -m "Menambahkan TP1 nomor 1 dan 2"
```

---

## 12. Push Branch

Push branch NIM ke repository fork:

```bash
git push origin NIM_ANDA
```

Contoh:

```bash
git push origin H071261041
```

Jika diminta:

```bash
git push --set-upstream origin H071261041
```

---

# 🔀 13. Membuat Pull Request

Setelah melakukan push:

1. Buka repository fork Anda di GitHub.
2. Klik **Compare & pull request**.
3. Pastikan target Pull Request benar.

### Base Repository

```text
OWNER/LAB-AP-18-2026
```

Branch:

```text
main
```

### Head Repository

```text
USERNAME_ANDA/LAB-AP-18-2026
```

Branch:

```text
NIM_ANDA
```

> **PENTING:** Base harus mengarah ke repository utama praktikum.

---

# 📝 14. Judul Pull Request

Gunakan format:

```text
[TP-<nomor>] <NIM> - <Nama Lengkap>
```

Contoh:

```text
[TP-1] H071261041 - Aisyah Kamila
```

---

# 📄 15. Deskripsi Pull Request

Gunakan format:

```md
## Identitas

- NIM: H071261041
- Nama: Aisyah Kamila
- Praktikum: 1

## Tugas

- TP1_1_H071261041.py
- TP1_2_H071261041.py
- TP1_3_H071261041.py

## Checklist

- [x] Program sudah diuji
- [x] Nama file sudah sesuai
- [x] Struktur folder sudah sesuai
- [x] Branch sudah menggunakan NIM
```

Kemudian klik:

```text
Create pull request
```

---

# 🔑 Autentikasi GitHub

Jika saat `git push` muncul:

```text
Username:
Password:
```

Gunakan:

```text
Username → Username GitHub Anda
Password → Personal Access Token (PAT)
```

> GitHub tidak lagi menerima password akun biasa untuk autentikasi Git melalui HTTPS.

## ⚠️ Keamanan PAT

Jangan pernah membagikan Personal Access Token kepada orang lain.

Jangan memasukkan token ke:

- Source code
- README
- Screenshot
- Commit
- Pull Request
- Repository publik
- Chat

---

# 🔄 Sinkronisasi Repository

Jika repository utama mengalami perubahan, sinkronkan repository fork sebelum mengerjakan tugas berikutnya.

Tambahkan repository utama sebagai `upstream`:

```bash
git remote add upstream https://github.com/OWNER/LAB-AP-18-2026.git
```

Cek:

```bash
git remote -v
```

Ambil perubahan:

```bash
git fetch upstream
```

Pindah ke `main`:

```bash
git checkout main
```

Gabungkan perubahan:

```bash
git merge upstream/main
```

Push ke fork:

```bash
git push origin main
```

Kemudian kembali ke branch NIM:

```bash
git checkout NIM_ANDA
```

---

# ⚠️ Aturan Penting

### 1. Jangan mengubah folder mahasiswa lain

Setiap mahasiswa hanya mengerjakan folder miliknya sendiri.

### 2. Jangan mengerjakan tugas pada branch `main`

Gunakan branch berdasarkan NIM.

### 3. Jangan menghapus file mahasiswa lain

Jangan menghapus atau memindahkan file tanpa instruksi dari asisten/dosen.

### 4. Gunakan format nama file yang benar

Benar:

```text
TP1_1_H071261041.py
```

Salah:

```text
soal1.py
tugas.py
TP1.py
TP1_1.py
```

### 5. Jangan mengupload file yang tidak diperlukan

Hindari:

```text
__pycache__/
*.pyc
.vscode/
.idea/
.DS_Store
```

---

# 📄 Contoh `.gitignore`

Buat file `.gitignore`:

```gitignore
__pycache__/
*.pyc

.vscode/
.idea/

.DS_Store
```

---

# 📂 Contoh Struktur Repository Akhir

```text
LAB-AP-18-2026/
│
├── H071261041 - Aisyah Kamila/
│   ├── Praktikum-1/
│   │   ├── TP1_1_H071261041.py
│   │   ├── TP1_2_H071261041.py
│   │   └── TP1_3_H071261041.py
│   │
│   ├── Praktikum-2/
│   │   ├── TP2_1_H071261041.py
│   │   └── TP2_2_H071261041.py
│   │
│   └── Praktikum-3/
│       └── TP3_1_H071261041.py
│
├── H071261042 - Abd. Faathir Ath Thaariq/
│   └── Praktikum-1/
│       └── TP1_1_H071261042.py
│
├── .gitignore
└── README.md
```

---

# 🧑‍💻 Ringkasan Perintah Git

```bash
# Clone
git clone https://github.com/USERNAME_ANDA/LAB-AP-18-2026.git

# Masuk repository
cd LAB-AP-18-2026

# Buat branch NIM
git checkout -b NIM_ANDA

# Cek status
git status

# Add
git add .

# Commit
git commit -m "Menambahkan tugas Praktikum 1"

# Push
git push origin NIM_ANDA
```

---

# 🆘 Troubleshooting

## Git tidak ditemukan

Jika muncul:

```text
command not found: git
```

Cek:

```bash
git --version
```

Pastikan Git sudah terinstal.

---

## Python tidak ditemukan

Coba:

```bash
python3 --version
```

Jika menggunakan `python3`:

```bash
python3 nama_file.py
```

---

## Salah Branch

Cek branch:

```bash
git branch
```

Pindah ke branch NIM:

```bash
git checkout NIM_ANDA
```

---

## Lupa `git add`

Jalankan:

```bash
git add .
```

Kemudian:

```bash
git commit -m "Menambahkan tugas"
```

---

## Push Ditolak

Pastikan:

1. Berada pada branch NIM.
2. Repository sudah di-fork.
3. `origin` mengarah ke repository fork.
4. Autentikasi GitHub sudah benar.

Cek:

```bash
git remote -v
```

---

# 📢 Catatan

Sebelum membuat Pull Request, pastikan:

- Nama folder sudah benar.
- Nama file sudah benar.
- Branch menggunakan NIM.
- Program sudah diuji.
- Tidak mengubah folder mahasiswa lain.
- Target Pull Request sudah benar.
- Base repository adalah repository utama `LAB-AP-18-2026`.

Kesalahan pada struktur repository atau Pull Request dapat menyebabkan tugas tidak dapat diproses dengan baik.

---

## 🎓 LAB-AP-18-2026

**Praktikum Algoritma & Pemrograman 2026**

**Happy Coding! 🚀**
