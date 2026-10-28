# Supervised Machine Learning: Regression
Tema: Reading Data — Game | Pemula | CSV + SQLite

Dataset sintetis berbeda dari proyek EDA sebelumnya. Penjualan hanya untuk latihan, bukan data industri nyata.

## Isi
- `data/game_sales_regression.csv`: 180 game dan target `sales_millions`.
- `data/player_feedback.csv`: 540 baris feedback.
- `data/game_sales.db`: SQLite berisi tabel `games`, `players`, `play_sessions`.
- `notebooks/01_Read_Game_Data.ipynb`: membaca CSV dan SQLite.
- `notebooks/02_Linear_Regression.ipynb`: regresi linear dan metrik.
- `notebooks/03_Train_Test_Split_and_Target.ipynb`: split dan transformasi target.
- `notebooks/04_Polynomial_Regression.ipynb`: polynomial regression.
- `notebooks/05_Cross_Validation_and_Regularization.ipynb`: cross-validation dan Ridge.
- `notebooks/06_LAB_Regression_Game.ipynb`: latihan mandiri.

## Setup VS Code Windows
Gunakan Python 3.13 64-bit untuk kompatibilitas paket; Python 3.15.2 boleh tetap terpasang. Unduh: https://www.python.org/downloads/release/python-3139/

1. Ekstrak ZIP dan buka folder proyek di VS Code.
2. Terminal → New Terminal, jalankan `py -3.13 -m venv .venv`.
3. Aktifkan dengan ` .\.venv\Scripts\Activate.ps1 `. Jika diblokir, jalankan `Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass`, lalu aktivasi lagi.
4. Jalankan `python -m pip install --upgrade pip` dan `python -m pip install -r requirements.txt`.
5. Buka notebook, pilih kernel `.venv`, lalu jalankan sel dari atas ke bawah.

Urutan belajar: notebook 01, 02, 03, 04, 05, lalu 06.
