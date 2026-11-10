# 📄 Laporan Proyek 3 — GaluraSwara

Repositori dokumen naskah **Laporan Proyek 3** (Sarjana Terapan Teknik Informatika - Universitas Logistik dan Bisnis Internasional / ULBI) untuk sistem **GaluraSwara**: *Aplikasi Pemutar Playlist dan Musik Tradisional*.

- 🌐 **Landing Page**: [https://galuraswara.github.io/](https://galuraswara.github.io/)
- 📱 **AndroidApp**: [GaluraSwara/AndroidApp](https://github.com/GaluraSwara/AndroidApp)
- ⚙️ **Backend**: [GaluraSwara/Backend](https://github.com/GaluraSwara/Backend)
- 📄 **API Docs**: [GaluraSwara/apidocs](https://galuraswara.github.io/apidocs/)

---

## 📚 Struktur Naskah LaTeX
Dokumen ini disusun menggunakan standar format penulisan akademik LaTeX dengan struktur:
- `main.tex`: Berkas induk LaTeX, metadata sampul, konfigurasi paket (Times New Roman, margin 4-3-3-3, format judul & daftar pustaka).
- `chapters/ringkasan.tex`: Ringkasan eksekutif / abstrak proyek.
- `chapters/bab1.tex`: Bab I Pendahuluan (Latar Belakang, Rumusan Masalah, Tujuan, Batasan).
- `chapters/bab2.tex`: Bab II Tinjauan Pustaka (Gocroot, MongoDB, Native Kotlin, Media3 ExoPlayer, Croot.js, CI/CD).
- `chapters/bab3.tex`: Bab III Perancangan Sistem (Arsitektur sistem, skema basis data, antarmuka pengguna, workflow DevOps).
- `chapters/bab4.tex`: Bab IV Implementasi dan Pengujian (Black box testing seluruh subsistem).
- `chapters/bab5.tex`: Bab V Kesimpulan dan Saran.
- `chapters/lampiran.tex`: Tautan repositori dan cuplikan konfigurasi workflow.

---

## 🤖 Otomatisasi CI/CD: Compile LaTeX, Auto Tag & GitHub Release
Repositori ini telah dilengkapi dengan GitHub Actions Workflow pada berkas [`.github/workflows/latex_release.yml`](.github/workflows/latex_release.yml).

Setiap kali dilakukan `git push` ke branch `main` atau `master`:
1. Dokumen LaTeX `main.tex` akan dikompilasi secara otomatis menjadi `main.pdf` menggunakan mesin `pdflatex`.
2. Git tag rilis dibuat secara otomatis dengan format inkremental (`v1.0.x`).
3. File PDF hasil kompilasi langsung diunggah ke tab **GitHub Releases** sebagai artefak siap unduh.

---

## 💻 Kompilasi Dokumen Secara Lokal
Bagi yang memiliki distribusi TeX (TeX Live, MiKTeX, atau MacTeX) di komputer lokal:

```bash
# Kompilasi pdflatex
pdflatex main.tex
pdflatex main.tex  # Jalankan dua kali untuk nomor halaman dan daftar isi
```
Atau dapat disunting langsung di platform editor kolaboratif seperti **Overleaf**.
