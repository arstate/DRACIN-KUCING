# 02. STRUKTUR & WORKFLOW PRODUKSI EPISODE
## Standar Operasional Produksi Serial Drama Vertikal (100 Episode)
### Format: Vertikal 9:16 | Durasi 120 Detik (2 Menit Pas) | Target Platform: TikTok & YouTube Shorts

---

## 🗺️ 1. ROADMAP 100 EPISODE (10 DRAMATIC ARCS)
Produksi serial drama vertikal ini dibagi ke dalam 10 Arc dramatis bertempo cepat, adiktif, dan sarat emosi balas dendam:

1. **Arc 1 (Eps 001 - 010): Penolakan di Pesta Grevy & Cincin 1,99 Triliun** (Oyen ditolak di pesta, kaleng mahar ditendang, Grevy menembak Molly dengan cincin 2g 1,99T, Oyen memerintahkan audit rahasia).
2. **Arc 2 (Eps 011 - 020): Transformasi Sikap Oyen & Kelakuan Playboy Grevy** (Oyen berubah dingin dan cuek, Grevy mulai berselingkuh di hotel bintang lima, pertemuan hangat dengan Cici di warung kelontong).
3. **Arc 3 (Eps 021 - 030): Perselingkuhan Grevy Terbongkar Basah** (Molly menggerebek Grevy di klub malam, terbongkar cincin 1,99T cuma emas loak sepuhan Rp 500rb, Molly diusir ke jalanan dan mencoba mengemis maaf ke Oyen kuli).
4. **Arc 4 (Eps 031 - 040): Inspeksi Rumah Mewah & Jatuhnya Grevy** (Oyen menuntaskan mega-mansion megahnya, Grevy terlilit utang dan mencoba membobol brankas proyek Oyen, persiapan Gala Peresmian Akbar).
5. **Arc 5 (Eps 041 - 050): The Grand Reveal — Sultan Membuka Kedok** (Oyen turun dengan jas bespoke kaisar emas hitam, Grevy dan Molly syok membatu, Grevy dipecat dan diborgol polisi, Molly merangkul kaki Oyen ditolak dingin).
6. **Arc 6 (Eps 051 - 060): Mahar 2,5 Juta Quintiliun & Penyerahan Rumah Mewah** (Oyen melamar Cici dengan cincin berlian 999,1 Quintiliun, mahar 2,5 Juta Quintiliun tunai, dan akta hibah Mega-Mansion).
7. **Arc 7 (Eps 061 - 070): Sabotase Keluarga Grevy & Pertahanan Cici** (Keluarga besar Grevy mencoba menggugat aset, keteguhan hati dan kecerdasan Cici membungkam para penggugat).
8. **Arc 8 (Eps 071 - 080): Kehancuran Mental Molly & Kehidupan Pengemis** (Molly jatuh miskin menjadi pengemis jalanan meratapi cincin palsu dan kebodohan masa lalunya).
9. **Arc 9 (Eps 081 - 090): Kelahiran Sang Putra Mahkota "Nico William bin Ochi"** (Cici melahirkan Nico William, kebahagiaan keluarga besar Kencana, perayaan akbar seluruh kota).
10. **Arc 10 (Eps 091 - 100): Puncak Kejayaan Imperium Kencana & Penyesalan Abadi** (Penobatan Nico William, pembersihan sisa koruptor kota, pesan moral ketulusan mengalahkan keserakahan, Molly menatap istana dari balik jeruji trotoar).

---

## ⏱️ 2. PACING DRAMATIS PER EPISODE (PETA WAKTU 120 DETIK)
Setiap episode dirancang presisi dengan 4 Scene terukur:

```text
[00:00 - 00:03] -> HOOK PEMBUKA KINETIK 3 DETIK (Snap Zoom / Suara Benturan Keras / Batin menusuk jiwa)
[00:03 - 00:30] -> SCENE 1: SETUP KONFLIK & FRICTION (Adegan pembuka memancing emosi penonton)
[00:30 - 00:60] -> SCENE 2: ESKALASI KETEGANGAN (Konfrontasi karakter / kontras visual tajam)
[00:60 - 00:90] -> SCENE 3: TITIK KRITIS & REVELATION (Fakta terungkap / dialog dramatis menusuk)
[00:90 - 01:20] -> SCENE 4: TITIK PUNCAK & MEGA-CLIFFHANGER MAUT (Detik 118-120: Hard Cut to Black + CTA)
```

---

## ⚡ 3. THE GOLDEN CLIFFHANGER RULE (ATURAN GANTUNG MAUT)
* **Larangan Menyelesaikan Masalah di Episode yang Sama:**
  Setiap akhir episode **DILARANG MEMBERI PENYELESAIAN (NO CLOSURE)**.
* **Titik Potong:**
  Potong video tepat di milidetik puncak ketegangan psikologis (misal: saat tamparan melayang di udara, saat suara petir menyambar di atas kata perintah Oyen, saat kotak cincin terbuka, saat borgol polisi berbunyi `KLIK`).
* **Layar Hitam CTA Provokatif (Detik Terakhir):**
  Layar hitam pekat selama 2-3 detik dengan teks merah/putih kontras tinggi yang memaksa penonton mem-follow akun TikTok dan subscribe YouTube:
  ```text
  "FOLLOW @kucingoyen.sultan SEKARANG UNTUK NONTON KELANJUTAN EPS XX!"
  ```

---

## 📂 4. STANDAR 6 FILE WAJIB PER FOLDER EPISODE (`S1_EPS_XX/`)
Setiap folder episode `S1_EPS_XX/` (misal `S1_EPS_01/`, `S1_EPS_02/`, dst.) WAJIB berisi 6 berkas operasional:

1. **`CERITA_NASKAH_EPS_XX.txt`:**
   Naskah cerita 120 detik, lengkap dengan dialog verbatim per detik, petunjuk SFX audio, deskripsi visual kamera, dan naskah mega-cliffhanger.
2. **`01_PROMPT_SCENE_LATAR.md`:**
   Prompt tunggal Nano Banana 2.1 untuk mengenerate latar/environment 4 scene (tanpa karakter).
3. **`02_PROMPT_KARAKTER_AKTOR_PER_SCENE.md`:**
   Prompt karakter aktor terisolasi di latar putih solid `#FFFFFF` f/8 untuk acuan karakter.
4. **`03_PROMPT_MASTER_SCENE_UTAMA.md`:**
   Prompt gabungan Master Scene definitif 1 s/d 4 (1 prompt per scene) dengan multi-image reference stack lengkap.
5. **`04_PROMPT_MULTISHOT_PER_SCENE.md`:**
   Prompt variasi multi-shot (4 sudut kamera: Wide, Medium, Close-Up, Special Angle) per scene dengan mewajibkan gambar master scene sebagai referensi utama (bobot `0.90`).
6. **`05_PROMPT_IMAGE_TO_VIDEO_MULTI_SHOT.md`:**
   Prompt video AI (Kling / Runway) dengan opsi durasi (4s/6s/8s/10s), gaya kamera handheld organik, dan panduan sinkronisasi dialog agar audio tidak terpotong.

---

## 🗂️ 5. SUBFOLDER OPERASIONAL PER SCENE
Di dalam folder episode, sediakan 4 subfolder scene (`SCENE_01/`, `SCENE_02/`, `SCENE_03/`, `SCENE_04/`), masing-masing berisi 5 subfolder eksekusi:

* `INPUT_REF_IMAGE/` -> Tempat menaruh file gambar referensi acuan sebelum digenerate.
* `HASIL_GEN_MASTER/` -> Tempat menyimpan gambar hasil generate master scene utama (`S1_SCENE_XX_MASTER.png`).
* `HASIL_GEN_MULTISHOT/` -> Tempat menyimpan gambar 4 sudut kamera multi-shot.
* `INPUT_REF_VIDEO/` -> Tempat menaruh 1 gambar terbaik yang akan di-upload ke mesin video AI.
* `HASIL_GEN_VIDEO/` -> Tempat menyimpan video akhir hasil render (`S1_SCENE_XX_VIDEO.mp4`).
* Plus 3 berkas mandiri per scene: `PROMPT_MASTER_SCENE_0X.md`, `PROMPT_MULTISHOT_SCENE_0X.md`, dan `PROMPT_VIDEO_SCENE_0X.md`.
