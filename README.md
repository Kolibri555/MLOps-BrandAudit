# Automated Influencer Integrity & Brand Safety Audit System

## Tujuan Proyek
Proyek ini adalah implementasi *Machine Learning Operations* (MLOps) untuk membangun sistem cerdas yang dapat mengaudit integritas *influencer* dan menjaga keamanan *brand* (*Brand Safety*). Sistem ini secara otomatis mendeteksi konten berisiko (seperti *hate speech*, konten toksik, atau aktivitas *bot*) menggunakan model *Natural Language Processing* (NLP) dan Google Gemini API, dilengkapi dengan kapabilitas *Continual Learning* untuk beradaptasi dengan perubahan bahasa (*Data/Concept Drift*).

## Struktur Direktori
Proyek ini diorganisasikan menggunakan standar industri (*Cookiecutter Data Science*) agar rapi, modular, dan mudah di-reproduksi:

- `config/` : Pengaturan konfigurasi sistem (target scraping, parameter model).
- `data/` : Penyimpanan data mentah (*raw*), data bersih (*processed*), dan *database* (SQLite/ChromaDB).
- `models/` : Direktori untuk menyimpan file model ML yang sudah dilatih (contoh: `.pkl`).
- `notebooks/` : Kumpulan Jupyter Notebook untuk keperluan eksplorasi data awal (EDA) dan eksperimen.
- `src/` : Kumpulan kode sumber (source code) utama yang siap masuk tahap produksi (ingestion, processing, intelligence, monitoring, API).
- `.devcontainer/` : Konfigurasi lingkungan kerja isolasi agar konsisten di GitHub Codespaces.

## Cara Menjalankan Lingkungan (Codespaces)
Proyek ini sudah dikonfigurasi sepenuhnya menggunakan **GitHub Codespaces** dengan spesifikasi Python 3.10 dan instalasi *library* otomatis (via `devcontainer.json`).

Langkah-langkah untuk menjalankan:
1. Buka halaman repositori GitHub ini.
2. Klik tombol hijau **`<> Code`**.
3. Pilih tab **`Codespaces`**.
4. Klik **`Create codespace on main`** (atau buka codespace yang sudah ada).
5. Tunggu proses *building container* selesai. Lingkungan kerja (termasuk semua *dependencies* di `requirements.txt`) akan otomatis terinstal dan siap digunakan secara instan tanpa perlu konfigurasi manual.