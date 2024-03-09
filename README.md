# Tugas-Besar-Strategi-Algoritma-2024-Jadi-Mesin - Pemanfaatan Algoritma Greedy dalam Pembuatan Bot Permainan Diamonds


<!--
i. Penjelasan singkat algoritma greedy yang diimplementasikan
ii. Requirement program dan instalasi tertentu bila ada
iii. Command atau langkah-langkah dalam meng-compile atau build
program
iv. Author (identitas pembuat)
-->

## Table of Contents

- [General Info](#general-information)
- [Team Members](#team-members)
- [How to Run](#how-to-run)
- [Program Structure](#program-structure)

## General Information

```
Pada tugas pertama Strategi Algoritma ini, dibuat sebuah bot yang nantinya akan dipertandingkan satu sama lain. Bot tersebut akan menggunakan strategi greedy dalam melakukan pergerakan. Secara singkat dan sederhana, strategi greedy yang kami gunakan adalah memilih diamond berdasarkan density terbesar. Pada kasus ini, density yang dimaksud adalah nilai bobot diamond dibagi dengan jarak diamond. Tentunya kami juga  memastikan bahwa diamond yang menjadi solusi harus bisa diambil dengan mempertimbangkan komponen-komponen game lain seperti bot musuh, tombol merah, base, dan teleportasi.

Berikut adalah deskripsi Program permainan Diamonds: 
1. Game engine, yang secara umum berisi: 
Kode backend permainan, yang berisi logic permainan secara keseluruhan serta API yang disediakan untuk berkomunikasi dengan frontend dan program bot 
Kode frontend permainan, yang berfungsi untuk memvisualisasikan permainan 

2. Bot starter pack, yang secara umum berisi: 
Program untuk memanggil API yang tersedia pada backend 
Program bot logic (bagian ini yang akan kalian implementasikan dengan algoritma greedy untuk bot kelompok kalian) 
Program utama (main) dan utilitas lainnya 
```

## How to Run

1. Pemasangan Persyaratan:

- Python 3 (https://www.python.org/downloads/)
- Node.js (https://nodejs.org/en)
- Docker desktop (https://www.docker.com/products/docker-desktop/)
- Yarn
  ```
  npm install --global yarn
  ```

2. Clone repository ini.

```
$ git clone https://github.com/PanjiSri/Tubes1_JadiMesin.git
```

3. Masuk ke root directory dari project.
```
cd tubes1-IF2110-game-engine-1.1.0
```

4. Install dependencies menggunakan Yarn.
```
yarn
```

5. Run initiate.pl with the argument below
   Untuk Windows
```
./scripts/copy-env.bat
```
   Untuk Linux / (possibly) macOS
```
chmod +x ./scripts/copy-env.sh
./scripts/copy-env.sh
```

6.  Setup local database (buka aplikasi docker desktop terlebih dahulu, lalu jalankan command berikut di terminal)
```
docker compose up -d database
```
   Untuk Windows
```
./scripts/setup-db-prisma.bat
```
   Untuk Linux / (possibly) macOS
```
chmod +x ./scripts/setup-db-prisma.sh
./scripts/setup-db-prisma.s
```
7. Build
```
npm run build
```
8. Run
```
npm run start
```
9. Masuk ke root directory dari projec
```
cd tubes1-IF2110-bot-starter-pack-1.0.1
```
10. Install dependencies menggunakan pip
```
pip install -r requirements.txt
```
11. Untuk menjalankan beberapa bot sekaligus (pada contoh ini, kita menjalankan 4 bot dengan logic yang sama, yaitu game/logic/random.py)
  Untuk windows
```
./run-bots.bat
```
  Untuk Linux / (possibly) macOS
```
./run-bots.sh
```

## Team Members

| **NIM**  |        **Nama**         |
| :------: | :---------------------: |
| 13521013 | Panji Sri Kuncara Wisma |
| 13521041 |   Ahmad Hasan Albana    |
| 13521042 |      Amalia Putri       |

## Program Structure

```
.
│   README.md
|
└───doc
|   └───Progress1_G03.pdf
|       Progress2_G03.pdf
|       Laporan_G03.pdf
|
└───src
    |
    └───attack.pl
        dynamicfacts.pl
        initiate.pl
        map.pl
        player.pl
        risk.pl
        rules.pl
        staticfacts.pl
        troops.pl
        turn.pl
        utilities.pl
        wilayah.pl
```
