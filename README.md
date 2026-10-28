# Exploratory Data Analysis for Machine Learning
## Tema: Reading Data — Game | Tingkat: Pemula | Format: CSV + SQLite

Proyek latihan dengan data **sintetis** (dibuat untuk pembelajaran, bukan data industri nyata).

## Isi folder
- `data/games_eda.csv` — katalog 80 game sintetis.
- `data/player_reviews.csv` — 240 ulasan pemain sintetis.
- `data/game_platform.db` — database SQLite berisi tabel `games`, `players`, dan `play_sessions`.
- `notebooks/01_Reading_Game_Data.ipynb` — membaca CSV dan SQLite.
- `notebooks/02_Exploratory_Data_Analysis.ipynb` — pemeriksaan data, statistik, grafik.
- `notebooks/03_Feature_Engineering_Game.ipynb` — membuat fitur sederhana.
- `notebooks/04_Hypothesis_Testing_Game.ipynb` — uji t Welch untuk latihan.

## Rekomendasi Python
Python 3.15.2 masih sangat baru, sehingga beberapa paket ilmiah mungkin belum menyediakan wheel yang cocok. Untuk pemula, gunakan **Python 3.13 64-bit** untuk proyek ini. Python 3.15 tetap boleh terpasang.

Unduh Python 3.13 dari:
https://www.python.org/downloads/release/python-3139/

## Langkah menjalankan di VS Code (Windows)
1. Ekstrak ZIP ke folder yang mudah ditemukan.
2. Buka VS Code → **File → Open Folder...** → pilih folder `Exploratory_Data_Analysis_for_Machine_Learning`.
3. Buka **Terminal → New Terminal**. Pastikan terminal berada di folder proyek yang memiliki `requirements.txt`.
4. Jika Python 3.13 sudah terpasang, buat virtual environment:
   ```powershell
   py -3.13 -m venv .venv
   ```
5. Aktifkan environment:
   ```powershell
   .\.venv\Scripts\Activate.ps1
   ```
   Jika PowerShell memblokir aktivasi, jalankan:
   ```powershell
   Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
   .\.venv\Scripts\Activate.ps1
   ```
6. Pasang paket:
   ```powershell
   python -m pip install --upgrade pip
   python -m pip install -r requirements.txt
   ```
7. Di VS Code, pasang ekstensi **Python** dan **Jupyter** jika belum ada.
8. Buka notebook di folder `notebooks`, pilih kernel yang menunjuk ke `.venv`, lalu jalankan sel dari atas ke bawah.

## Jika hanya Python 3.15 yang terpasang
Jangan hapus Python 3.15. Pasang Python 3.13 berdampingan. Setelah itu jalankan `py -0p` untuk memastikan versi 3.13 muncul.

## Catatan
- Semua data dibuat secara acak dengan seed tetap agar hasil dataset konsisten saat ZIP dibuat.
- Tidak diperlukan koneksi internet untuk membaca dataset setelah paket Python terpasang.
- Untuk `04_Hypothesis_Testing_Game.ipynb`, SciPy disertakan dalam requirements.
