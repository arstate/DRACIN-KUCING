# 05. STRUKTUR FOLDER & MANAJEMEN ASET
## Konvensi Direktori dan Pengelolaan Aset Produksi Serial Drama Vertikal

---

## 🌳 1. PETA POHON STRUKTUR DIREKTORI REPOSITORI

```text
/mnt/HDD-2/BACKUP LINUX/FILE DATA/DRACIN KUCING/
├── README.md                               <-- Panduan landing page GitHub (System Prompt AI Agent)
├── README_MASTER_PRODUKSI.md               <-- Master dokumentasi root
├── 00_ROADMAP_100_EPISODE_SULTAN_KULI.md   <-- Master Roadmap 100 Episode lengkap (10 Arc)
│
├── README AI AGENT/                        <-- [SSOT] Seluruh panduan operasional AI Agent
│   ├── 00_README_MASTER_AGENTS.md
│   ├── 01_KONSEP_CERITA_DAN_LORE_UNIVERSE.md
│   ├── 02_STRUKTUR_DAN_WORKFLOW_PRODUKSI_EPISODE.md
│   ├── 03_STANDAR_PROMPT_IMAGE_NANO_BANANA_2_1.md
│   ├── 04_STANDAR_PROMPT_IMAGE_TO_VIDEO_IMG2VID.md
│   ├── 05_STRUKTUR_FOLDER_DAN_MANAJEMEN_ASET.md
│   └── 06_PANDUAN_OPERASIONAL_AI_AGENT_BARU.md
│
├── ASET_KARAKTER_SULTAN_KULI/              <-- Library Pecahan Modular Prompt Karakter Baru
│   ├── MASTER_PROMPT_KARAKTER_SULTAN_KULI.md <-- Panduan karakter gabungan
│   ├── 01_OYEN_KULI_DAN_SULTAN.md          <-- Oyen mode kuli vs mode sultan
│   ├── 02_MOLLY_MATRE.md                   <-- Molly Calico gaun hot-pink
│   ├── 03_GREVY_PLAYBOY.md                 <-- Grevy Bombay jas pinstripe & cerutu
│   ├── 04_CICI_TULUS.md                    <-- Cici Persia putih gaun pastel toko
│   ├── 05_NICO_WILLIAM.md                  <-- Nico William putra mahkota beludru navy
│   └── 06_PROPERTI_IKONIK.md               <-- Kaleng mahar, Cincin 1,99T, Cincin 999,1Q, Ponsel satelit
│
├── S1_EPS_01/                              <-- Folder Produksi Episode 01
│   ├── CERITA_NASKAH_EPS_01.txt           <-- Naskah narasi & dialog 120 detik (SATU-SATUNYA FILE DI ROOT EPS)
│   │
│   ├── SCENE_01/                          <-- Eksekusi Modular Scene 01
│   │   ├── 01_PROMPT_LATAR_SCENE_01.md     <-- Prompt Latar/Environment
│   │   ├── 02_PROMPT_KARAKTER_SCENE_01.md  <-- Prompt Aktor terisolasi putih
│   │   ├── 03_PROMPT_MASTER_SCENE_01.md    <-- Prompt Master Scene Utama
│   │   ├── 04_PROMPT_MULTISHOT_SCENE_01.md <-- Prompt 4 Sudut Kamera
│   │   ├── 05_PROMPT_VIDEO_SCENE_01.md     <-- Prompt Img2Vid & audio sync
│   │   ├── INPUT_REF_IMAGE/               <-- Drop gambar referensi input user di sini
│   │   ├── HASIL_GEN_MASTER/              <-- Simpan S1_SCENE_01_MASTER.png di sini
│   │   ├── HASIL_GEN_MULTISHOT/           <-- Simpan hasil generate 4 shot di sini
│   │   ├── INPUT_REF_VIDEO/               <-- Drop S1_SCENE_01_REF_FOR_VIDEO.png di sini
│   │   └── HASIL_GEN_VIDEO/               <-- Simpan S1_SCENE_01_VIDEO.mp4 di sini
│   │
│   ├── SCENE_02/                          <-- Eksekusi Modular Scene 02 (struktur sama: 5 file prompt + 5 folder)
│   ├── SCENE_03/                          <-- Eksekusi Modular Scene 03 (struktur sama: 5 file prompt + 5 folder)
│   └── SCENE_04/                          <-- Eksekusi Modular Scene 04 (struktur sama: 5 file prompt + 5 folder)
│
├── S1_EPS_02/                             <-- Folder Produksi Episode 02 (CERITA_NASKAH_EPS_02.txt)
├── ...
└── S1_EPS_10/                             <-- Folder Produksi Episode 10
```

---

## 🏷️ 2. KONVENSI PENAMAAN FILE (FILE NAMING CONVENTIONS)

Gunakan format baku berikut agar file tidak tertukar di editor video atau sistem AI:

### A. Berkas Prompt di Dalam Folder Scene:
* `01_PROMPT_LATAR_SCENE_{NomorScene}.md`
* `02_PROMPT_KARAKTER_SCENE_{NomorScene}.md`
* `03_PROMPT_MASTER_SCENE_{NomorScene}.md`
* `04_PROMPT_MULTISHOT_SCENE_{NomorScene}.md`
* `05_PROMPT_VIDEO_SCENE_{NomorScene}.md`

### B. Gambar Master Scene Utama:
* `S{Season}_SCENE_{NomorScene}_MASTER.png`
* *Contoh:* `S1_SCENE_01_MASTER.png`, `S1_SCENE_02_MASTER.png`

### C. Gambar Multi-Shot Sudut Kamera:
* `S{Season}_SCENE_{NomorScene}_SHOT_{NomorShot}_{JenisAngle}.png`
* *Contoh:*
  * `S1_SCENE_01_SHOT_01_WIDE.png`
  * `S1_SCENE_01_SHOT_02_MEDIUM.png`
  * `S1_SCENE_01_SHOT_03_CLOSEUP.png`
  * `S1_SCENE_01_SHOT_04_LOWANGLE.png`

### D. Gambar Input Mesin Video (First-Frame Image):
* `S{Season}_SCENE_{NomorScene}_REF_FOR_VIDEO.png`
* *Contoh:* `S1_SCENE_01_REF_FOR_VIDEO.png`

### E. File Video Akhir (.mp4):
* `S{Season}_SCENE_{NomorScene}_VIDEO.mp4`
* *Contoh:* `S1_SCENE_01_VIDEO.mp4`, `S1_SCENE_04_VIDEO.mp4`

---

## 💾 3. ATURAN PENYIMPANAN & HIGIENE WORKSPACE
1. **Dilarang Menaruh File Prompt di Root Episode:**
   Root folder episode (`S1_EPS_XX/`) HANYA boleh berisi naskah (`CERITA_NASKAH_EPS_XX.txt`) dan 4 folder scene. Semua prompt WAJIB berada di dalam masing-masing folder scene (`SCENE_01` s/d `SCENE_04`).
2. **Pemisahan Folder Ref & Hasil:**
   Jangan mencampur gambar referensi input dengan gambar hasil generate. Selalu simpan ke folder masing-masing (`INPUT_REF_*` vs `HASIL_GEN_*`) agar pengguna dapat bekerja manual dengan mudah dan rapi.
