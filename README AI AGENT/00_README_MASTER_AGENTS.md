# 🏢 MASTER ONBOARDING & ARCHITECTURE BIBLE: "KUCING OYEN SANG SULTAN KULI"
## Direktori Panduan Utama Sistem Produksi AI Agent (Multi-Agent Handover Bible)
### Target Format: Serial Drama Vertikal TikTok & YouTube Shorts (100 Episode @ 1–2 Menit)

> [!IMPORTANT]
> **PANDUAN UNTUK SEMUA AI AGENT (CLAUDE, GPT, GEMINI, DEEPSEEK, DLL):**
> Dokumen di dalam folder `README AI AGENT/` ini adalah **Single Source of Truth (SSOT)** dan pedoman operasional tertinggi. Setiap kali Anda (AI Agent) ditugaskan untuk melanjutkan, merevisi, atau membuat episode baru di proyek ini, Anda **WAJIB MEMBACA DAN MEMATUHI SELURUH STANDAR DI DALAM FOLDER INI**.

---

## 🧭 DAFTAR ISI DOKUMEN SISTEM (`README AI AGENT/`)

| Berkas Panduan | Deskripsi & Fokus Pembahasan |
| :--- | :--- |
| **[`00_README_MASTER_AGENTS.md`](file:///mnt/HDD-2/BACKUP%20LINUX/FILE%20DATA/DRACIN%20KUCING/README%20AI%20AGENT/00_README_MASTER_AGENTS.md)** | Ikhtisar eksekutif, aturan emas multi-agent, dan navigasi utama. |
| **[`01_KONSEP_CERITA_DAN_LORE_UNIVERSE.md`](file:///mnt/HDD-2/BACKUP%20LINUX/FILE%20DATA/DRACIN%20KUCING/README%20AI%20AGENT/01_KONSEP_CERITA_DAN_LORE_UNIVERSE.md)** | Lore semesta kucing Indonesia, plot Season 1, profil karakter biologis & properti nominal fixed. |
| **[`02_STRUKTUR_DAN_WORKFLOW_PRODUKSI_EPISODE.md`](file:///mnt/HDD-2/BACKUP%20LINUX/FILE%20DATA/DRACIN%20KUCING/README%20AI%20AGENT/02_STRUKTUR_DAN_WORKFLOW_PRODUKSI_EPISODE.md)** | Struktur 6 berkas per episode, pembagian 4 scene, durasi 120 detik, dan Golden Cliffhanger Rule. |
| **[`03_STANDAR_PROMPT_IMAGE_NANO_BANANA_2_1.md`](file:///mnt/HDD-2/BACKUP%20LINUX/FILE%20DATA/DRACIN%20KUCING/README%20AI%20AGENT/03_STANDAR_PROMPT_IMAGE_NANO_BANANA_2_1.md)** | Standar prompt gambar Nano Banana 2.1: optik f/8 no bokeh, negative prompt terpisah, master seed, dan multi-reference stack. |
| **[`04_STANDAR_PROMPT_IMAGE_TO_VIDEO_IMG2VID.md`](file:///mnt/HDD-2/BACKUP%20LINUX/FILE%20DATA/DRACIN%20KUCING/README%20AI%20AGENT/04_STANDAR_PROMPT_IMAGE_TO_VIDEO_IMG2VID.md)** | Standar prompt video AI (Kling/Runway), kamera handheld organik, opsi durasi 4s/6s/8s/10s, dan sinkronisasi dialog. |
| **[`05_STRUKTUR_FOLDER_DAN_MANAJEMEN_ASET.md`](file:///mnt/HDD-2/BACKUP%20LINUX/FILE%20DATA/DRACIN%20KUCING/README%20AI%20AGENT/05_STRUKTUR_FOLDER_DAN_MANAJEMEN_ASET.md)** | Struktur hierarki direktori, subfolder operasional per scene (`INPUT_REF`, `HASIL_GEN`), dan naming convention. |
| **[`06_PANDUAN_OPERASIONAL_AI_AGENT_BARU.md`](file:///mnt/HDD-2/BACKUP%20LINUX/FILE%20DATA/DRACIN%20KUCING/README%20AI%20AGENT/06_PANDUAN_OPERASIONAL_AI_AGENT_BARU.md)** | SOP teknis step-by-step untuk AI Agent yang baru mengambil alih sesi untuk memproduksi episode selanjutnya. |

---

## ⚡ 3 ATURAN EMAS NON-NEGOTIABLE (GOLDEN DIRECTIVES)

1. **ZERO DATA GUESSING (PANTANG MENGARANG DATA/LORE YANG SUDAH STATED):**
   - Karakter, nominal, dan alur cerita telah dikunci secara eksplisit oleh pengguna:
     * Oyen adalah Sultan Besar Kencana Imperium yang menyamar jadi kuli di proyek **Mega-Mansion** miliknya untuk mengetes ketulusan pasangan.
     * Grevy adalah Kucing Hitam Bombay CEO playboy bawahan Oyen yang korup. Grevy menembak Molly dengan **Cincin Emas 2 Gram seharga Rp 1,99 Triliun** (yang aslinya cincin sepuhan Rp 500rb dan korupsi proyek Oyen).
     * Molly adalah kucing Calico matre yang menolak Oyen kuli di pesta keluarga Grevy, menendang kaleng mahar Oyen, lalu menerima Grevy demi cincin 1,99T.
     * Cici adalah kucing Persia putih anggun penjaga warung kelontong yang menerima Oyen kuli apa adanya secara tulus.
     * Lamaran Akbar Oyen untuk Cici: **Cincin Berlian 999,1 Quintiliun**, **Mahar 2,5 Juta Quintiliun**, dan penyerahan istana **Mega-Mansion**.
     * Anak Oyen dan Cici bernama: **Nico William bin Ochi**.
   - Dilarang mengubah nama karakter, nominal, atau esensi cerita ini!

2. **ANTI-AI-SLOP & FOTOREALISTIS MUTLAK (NANO BANANA 2.1):**
   - Seluruh prompt gambar diam WAJIB menggunakan spesifikasi optik nyata: `Canon EOS R5, 35mm/50mm/85mm lens at f/8, deep depth of field, edge-to-edge tack-sharp focus, zero blurry bokeh, zero 3D render, zero CGI cartoon slop, Kodak Vision3 500T 35mm film grain, Aspect ratio 9:16 vertical portrait`.
   - Parameter `Negative Prompt` WAJIB ditaruh di blok/kolom terpisah di bawah prompt utama, DILARANG mencampurkan kata larangan ke bodi teks utama.

3. **GOLDEN CLIFFHANGER HOOK PADA DETIK TERAKHIR SETIAP EPISODE:**
   - Serial drama vertikal bergantung pada retensi dan konversi penonton menjadi followers.
   - Setiap episode (1–2 menit) **WAJIB DIGANTUNG CERITANYA PADA PUNCAK KETEGANGAN** (Detik 58–60 untuk durasi 1 menit, atau Detik 118–120 untuk durasi 2 menit).
   - Diakhiri dengan **HARD CUT TO BLACK** mendadak + Teks Layar Gelap Provokatif: `"FOLLOW @kucingoyen.sultan SEKARANG UNTUK NONTON KELANJUTAN EPISODE BERIKUTNYA!"`.
