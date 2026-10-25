# 06. PANDUAN OPERASIONAL AI AGENT BARU (HANDOVER PROTOCOL)
## Prosedur Standar Pengambilalihan Tugas (SOP Onboarding AI Agent)

> [!IMPORTANT]
> **JIKA ANDA ADALAH AI AGENT BARU YANG BARU MEMULAI SESI:**
> Baca dokumen ini terlebih dahulu sebelum membalas pesan pengguna atau membuat file apapun. Ikuti protokol 4 tahap di bawah ini secara ketat.

---

## 📋 TAHAP 1: PRE-FLIGHT AUDIT (BACA KONTEKS & CEK STATUS)
Sebelum menulis satu baris prompt pun:
1. **Verifikasi Lore Kunci:** Buka [`01_KONSEP_CERITA_DAN_LORE_UNIVERSE.md`](file:///mnt/HDD-2/BACKUP%20LINUX/FILE%20DATA/DRACIN%20KUCING/README%20AI%20AGENT/01_KONSEP_CERITA_DAN_LORE_UNIVERSE.md). Hafalkan nama tokoh (Oyen/Ochi, Molly, Grevy, Cici, Nico William) dan nominal aset (Cincin 2g 1,99T palsu Grevy, Cincin Berlian 999,1 Quintiliun, Mahar 2,5 Juta Quintiliun, Mega-Mansion).
2. **Cek Posisi Roadmap:** Buka [`00_ROADMAP_100_EPISODE_SULTAN_KULI.md`](file:///mnt/HDD-2/BACKUP%20LINUX/FILE%20DATA/DRACIN%20KUCING/00_ROADMAP_100_EPISODE_SULTAN_KULI.md). Lihat episode berapa yang sedang dikerjakan dan apa sinopsisnya.
3. **Cek Episode Sebelumnya:** Buka naskah episode sebelumnya untuk memastikan kontinuitas emosi dan adegan tidak melompat.

---

## 🛠️ TAHAP 2: EKSEKUSI PRODUKSI EPISODE BARU (STEP-BY-STEP)
Ketika pengguna meminta membuat episode baru (misal: "Buatkan Episode 02", "Lanjut Episode 03", dst.):

### 1. Buat Naskah Lengkap (`CERITA_NASKAH_EPS_XX.txt`)
* Durasi wajib **2 Menit (120 Detik Vertikal 9:16)**.
* Wajib ada:
  * Hook kinetik 3 detik pembuka.
  * Pembagian waktu per detik (Scene 1: 00:03-00:30, Scene 2: 00:30-00:60, Scene 3: 00:60-00:90, Scene 4: 00:90-01:20).
  * Dialog verbatim per detik (agar sinkron saat video AI di-generate).
  * **Mega-Cliffhanger Gantung Maut** di detik 118-120: Hard cut to black di puncak ketegangan + CTA Follow TikTok & Subscribe YouTube.

### 2. Buat 5 Berkas Panduan Global Episode:
* `01_PROMPT_SCENE_LATAR.md` (4 prompt latar tanpa karakter, optik f/8 no bokeh).
* `02_PROMPT_KARAKTER_AKTOR_PER_SCENE.md` (Aktor terisolasi latar putih `#FFFFFF`).
* `03_PROMPT_MASTER_SCENE_UTAMA.md` (1 prompt master per scene + panduan multi-reference).
* `04_PROMPT_MULTISHOT_PER_SCENE.md` (4 sudut kamera per scene: Wide, Medium, Close-Up, Special Angle; dengan gambar master scene sebagai Primary Reference bobot `0.90`).
* `05_PROMPT_IMAGE_TO_VIDEO_MULTI_SHOT.md` (Prompt Img2Vid Kling/Runway, kamera handheld organik, opsi durasi 4s/6s/8s/10s, dan sinkronisasi audio dialog).

### 3. Buat Folder & Berkas Per Scene (`SCENE_01` s/d `SCENE_04`):
Di dalam masing-masing folder scene:
* Buat 5 subfolder: `INPUT_REF_IMAGE/`, `HASIL_GEN_MASTER/`, `HASIL_GEN_MULTISHOT/`, `INPUT_REF_VIDEO/`, `HASIL_GEN_VIDEO/`.
* Buat 3 berkas eksekusi mandiri 1-prompt copas:
  * `PROMPT_MASTER_SCENE_0X.md`
  * `PROMPT_MULTISHOT_SCENE_0X.md`
  * `PROMPT_VIDEO_SCENE_0X.md`

---

## 🔍 TAHAP 3: VERIFIKASI POST-FLIGHT (QUALITY GATE CHECKLIST)
Sebelum menyerahkan hasil ke pengguna, pastikan 5 syarat kelulusan terpenuhi:
- [ ] **Optik Kamera Terkunci:** Seluruh prompt gambar memakai `Canon EOS R5 at f/8, deep depth of field, zero blurry bokeh, Kodak Vision3 500T 35mm grain, 9:16`.
- [ ] **Pemisahan Negative Prompt:** Parameter negatif tidak bercampur di bodi utama prompt.
- [ ] **Konsistensi Seed:** Menggunakan master seed baku (`8849201` untuk Oyen, `5528301` untuk Molly, `6639402` untuk Grevy, `7740503` untuk Cici).
- [ ] **Cliffhanger Ending:** Episode diakhiri dengan cut-to-black gantung di detik akhir (bukan resolusi damai).
- [ ] **Integritas Folder:** Subfolder `INPUT_REF_*` dan `HASIL_GEN_*` tersedia di tiap scene.

---

## 🧠 TAHAP 4: HUKUM CO-FOUNDER & ANTI-YES-MAN
Sebagai AI Agent profesional:
1. **Koreksi Jika Berisiko Kurang Menjual:** Jika pengguna meminta adegan yang membosankan, lambat, atau merusak retensi penonton TikTok/Shorts, berikan masukan kritis secara terbuka dan tawarkan alternatif adegan yang lebih dramatis dan adiktif.
2. **Jaga Konsistensi Format:** Jangan kembali ke format prompt bertele-tele atau prompt multi-agent kompleks. Pengguna mengenerate secara manual menggunakan **Nano Banana 2.1** (1 Prompt 1 Aksi Copas).
3. **Respon Terse & Padat:** Jawab langsung ke poin, laporkan file apa saja yang dibuat/diubah, dan tanyakan langkah selanjutnya secara proaktif.
