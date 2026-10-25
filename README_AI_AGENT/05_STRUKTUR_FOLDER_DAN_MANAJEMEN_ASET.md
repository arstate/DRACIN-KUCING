# 05. STRUKTUR FOLDER & MANAJEMEN ASET
## Konvensi Direktori dan Pengelolaan Aset Produksi Serial Drama Vertikal

---

## 🌳 1. PETA POHON STRUKTUR DIREKTORI REPOSITORI

```text
/mnt/HDD-2/BACKUP LINUX/FILE DATA/DRACIN KUCING/
├── README AI AGENT/                        <-- [SSOT] Seluruh panduan operasional AI Agent
│   ├── 00_README_MASTER_AGENTS.md
│   ├── 01_KONSEP_CERITA_DAN_LORE_UNIVERSE.md
│   ├── 02_STRUKTUR_DAN_WORKFLOW_PRODUKSI_EPISODE.md
│   ├── 03_STANDAR_PROMPT_IMAGE_NANO_BANANA_2_1.md
│   ├── 04_STANDAR_PROMPT_IMAGE_TO_VIDEO_IMG2VID.md
│   ├── 05_STRUKTUR_FOLDER_DAN_MANAJEMEN_ASET.md
│   └── 06_PANDUAN_OPERASIONAL_AI_AGENT_BARU.md
│
├── 00_ROADMAP_100_EPISODE_SULTAN_KULI.md  <-- Master Roadmap 100 Episode lengkap (10 Arc)
│
├── ASET_KARAKTER_SULTAN_KULI/              <-- Aset visual karakter dasar & properti kunci
│   └── MASTER_PROMPT_KARAKTER_SULTAN_KULI.md
│
├── S1_EPS_01/                              <-- Folder Produksi Episode 01
│   ├── CERITA_NASKAH_EPS_01.txt           <-- Naskah narasi & dialog 120 detik
│   ├── 01_PROMPT_SCENE_LATAR.md           <-- Prompt gambar latar 4 scene
│   ├── 02_PROMPT_KARAKTER_AKTOR_PER_SCENE.md <-- Prompt aktor terisolasi putih
│   ├── 03_PROMPT_MASTER_SCENE_UTAMA.md    <-- Prompt 4 master scene utama
│   ├── 04_PROMPT_MULTISHOT_PER_SCENE.md   <-- Prompt multishot variasi sudut kamera
│   ├── 05_PROMPT_IMAGE_TO_VIDEO_MULTI_SHOT.md <-- Prompt Img2Vid & audio timing
│   │
│   ├── SCENE_01/                          <-- Eksekusi Mandiri Scene 01
│   │   ├── PROMPT_MASTER_SCENE_01.md
│   │   ├── PROMPT_MULTISHOT_SCENE_01.md
│   │   ├── PROMPT_VIDEO_SCENE_01.md
│   │   ├── INPUT_REF_IMAGE/               <-- Drop gambar referensi input user di sini
│   │   ├── HASIL_GEN_MASTER/              <-- Simpan S1_SCENE_01_MASTER.png di sini
│   │   ├── HASIL_GEN_MULTISHOT/           <-- Simpan hasil generate 4 shot di sini
│   │   ├── INPUT_REF_VIDEO/               <-- Drop S1_SCENE_01_REF_FOR_VIDEO.png di sini
│   │   └── HASIL_GEN_VIDEO/               <-- Simpan S1_SCENE_01_VIDEO.mp4 di sini
│   │
│   ├── SCENE_02/                          <-- Eksekusi Mandiri Scene 02 (struktur sama)
│   ├── SCENE_03/                          <-- Eksekusi Mandiri Scene 03 (struktur sama)
│   └── SCENE_04/                          <-- Eksekusi Mandiri Scene 04 (struktur sama)
│
├── S1_EPS_02/                             <-- Folder Produksi Episode 02 (Batch 1)
├── S1_EPS_03/                             <-- Folder Produksi Episode 03 (Batch 1)
├── ...
└── S1_EPS_10/                             <-- Folder Produksi Episode 10 (Batch 1)
```

---

## 🏷️ 2. KONVENSI PENAMAAN FILE (FILE NAMING CONVENTIONS)

Gunakan format baku berikut agar file tidak tertukar di editor video atau sistem AI:

### A. Gambar Master Scene Utama:
* `S{Season}_SCENE_{NomorScene}_MASTER.png`
* *Contoh:* `S1_SCENE_01_MASTER.png`, `S1_SCENE_02_MASTER.png`

### B. Gambar Multi-Shot Sudut Kamera:
* `S{Season}_SCENE_{NomorScene}_SHOT_{NomorShot}_{JenisAngle}.png`
* *Contoh:*
  * `S1_SCENE_01_SHOT_01_WIDE.png`
  * `S1_SCENE_01_SHOT_02_MEDIUM.png`
  * `S1_SCENE_01_SHOT_03_CLOSEUP.png`
  * `S1_SCENE_01_SHOT_04_LOWANGLE.png`

### C. Gambar Input Mesin Video (First-Frame Image):
* `S{Season}_SCENE_{NomorScene}_REF_FOR_VIDEO.png`
* *Contoh:* `S1_SCENE_01_REF_FOR_VIDEO.png`

### D. File Video Akhir (.mp4):
* `S{Season}_SCENE_{NomorScene}_VIDEO.mp4`
* *Contoh:* `S1_SCENE_01_VIDEO.mp4`, `S1_SCENE_04_VIDEO.mp4`

---

## 💾 3. ATURAN PENYIMPANAN & HIGIENE WORKSPACE
1. **Dilarang Menghapus File Riwayat:**
   Seluruh berkas naskah (`.txt`) dan panduan prompt (`.md`) yang telah terverifikasi tidak boleh ditimpa atau dihapus oleh draft acak.
2. **Pemisahan Folder Ref & Hasil:**
   Jangan mencampur gambar referensi input dengan gambar hasil generate. Selalu pisahkan ke folder masing-masing (`INPUT_REF_*` vs `HASIL_GEN_*`) agar pengguna dapat bekerja manual dengan mudah dan rapi.
