# 03. STANDAR PROMPT IMAGE NANO BANANA 2.1
## Pedoman Prompting Fotorealistis Anti-AI-Slop (Aspect Ratio 9:16 Vertikal)

---

## 📷 1. MASTER KAMERA & OPTIK (THE ZERO-BOKEH MANDATE)
Untuk menghasilkan gambar yang tampak seperti rekaman film dokumenter nyata (bukan kartun 3D atau CGI buatan AI murahan), seluruh prompt Nano Banana 2.1 **WAJIB MENYERTAKAN PARAMETER OPTIK BERIKUT**:

* **Kamera:** `Canon EOS R5` (atau `ARRI Alexa Mini LF`).
* **Lensa:** `35mm` (Wide/Medium), `50mm` (Dynamic Action), `85mm` (Portrait/Close-Up), `100mm Macro` (Detail Perhiasan/Prop).
* **Aperture (Bukaan Diafragma):** `f/8` (atau `f/11` untuk Macro).
* **Depth of Field:** `Deep depth of field, edge-to-edge tack-sharp focus, zero artificial blurry bokeh`.
* **Tekstur Film:** `Kodak Vision3 500T 35mm motion picture film grain, subtle halation on light sources`.
* **Aspect Ratio:** `9:16 vertical portrait` (1080x1920 / vertikal smartphone).

> [!CAUTION]
> **BAHAYA ARTIFICIAL BOKEH:**
> Model AI difusi secara default gemar memburamkan latar belakang (*shallow depth of field / f/1.4 blur*). Ini membuat hasil tampak seperti miniatur mainan atau CGI murahan. Parameter `at f/8, deep depth of field, sharp focus from foreground to background, zero blurry bokeh` adalah pagar pelindung mutlak!

---

## ⛔ 2. STRUKTUR PEMISAHAN NEGATIVE PROMPT (ANTI-HALUSINASI)
* **Aturan Mutlak:** **DILARANG MENCAMPURKAN KATA LARANGAN KE DALAM BODI PROMPT UTAMA!**
  * *Salah:* "A cat without human face and not cartoon" -> Model AI justru membaca kata "human" dan "cartoon" sebagai target difusi!
  * *Benar:* Tulis deskripsi positif di bodi utama prompt, lalu masukkan kata terlarang ke dalam parameter/kolom **Negative Prompt** terpisah!

### Standar Baku Negative Prompt Nano Banana 2.1:
```text
human face, human skin, human hands, human fingers, 3d render, cgi, cartoon, anime, illustration, digital painting, doll plastic skin, airbrushed textures, flat lighting, blurry background, shallow depth of field, artificial bokeh, soft focus blur, deformed anatomy, extra paws, missing tail, text overlay, typography, watermark, logo.
```

---

## 🔢 3. MASTER SEED KONSISTENSI KARAKTER
Gunakan seed tetap berikut di Nano Banana 2.1 untuk mengunci struktur tulang, proporsi wajah, dan corak bulu karakter:

| Karakter / Aset | Master Seed Resmi | Ciri Khas Biologis & Kostum Terkunci |
| :--- | :--- | :--- |
| **Oyen / Ochi** | `8849201` | Bulu oren belang marmalade, mata tembaga-amber, luka notch di ujung telinga kiri, tubuh atletis kekar. |
| **Molly** | `5528301` | Kucing Calico belang tiga, mata hijau dengan riasan eyeliner hitam menor tebal, gaun mini satin hot-pink ketat. |
| **Grevy** | `6639402` | Kucing Bombay hitam legam mengkilap, mata kuning amber licik, seringai taring tajam, jas pinstripe arang & cerutu. |
| **Cici** | `7740503` | Kucing Persia putih murni halus, mata biru safir jernih berbinar tulus, gaun katun floral pastel & celemek linen. |
| **Nico William** | `9951604` | Anak kucing persilangan bulu putih berbelang marmalade halus, mata biru-amber, setelan beludru navy mini. |
| **Latar Environment** | `9928101` | Arsitektur metropolitan Indonesia realistis f/8. |

---

## 🔄 4. SOP MULTI-IMAGE REFERENCE STACK (KONSISTENSI 100%)

Untuk menghasilkan adegan yang nyambung antar-scene dan variasi multi-shot yang tidak berubah kostumnya, jalankan alur 4 langkah berikut:

### Step 1: Latar Environment
* Generate latar lokasi tanpa ada karakter (misal: pelataran karpet merah pesta, jalanan hujan, atau gerbang mega-mansion).
* Simpan sebagai referensi latar (`REF_LATAR_SCENE_XX.png`).

### Step 2: Aktor Terisolasi Latar Putih (`#FFFFFF`)
* Generate karakter terisolasi di latar putih solid studio light box f/8.
* Ini menghasilkan "kartu identitas visual" karakter dengan detail bulu dan pakaian yang bersih.

### Step 3: Master Scene Utama (Satu Prompt Definitif)
* Di panel Image Reference Nano Banana 2.1, upload:
  1. File Latar dari Step 1.
  2. File Aktor dari Step 2.
  3. File Prop Kunci (misal: kaleng mahar, kotak cincin emas 2 gram, atau ponsel satelit emas).
* Jalankan prompt Master Scene untuk mendapatkan **SATU GAMBAR DEFINITIF** adegan tersebut.
* Simpan hasilnya ke: `HASIL_GEN_MASTER/S1_SCENE_XX_MASTER.png`.

### Step 4: Multi-Shot Variasi Sudut Kamera (Bobot `0.90`)
* Saat mengenerate variasi sudut kamera (Shot 1 Wide, Shot 2 Medium, Shot 3 Close-Up, Shot 4 Special Angle):
  * **WAJIB MENG-UPLOAD GAMBAR HASIL MASTER SCENE (`S1_SCENE_XX_MASTER.png`) SEBAGAI PRIMARY REFERENCE DENGAN BOBOT TINGGI `0.90`!**
  * Trik ini menjamin bahwa saat kamera berpindah sudut (misal dari Wide ke Close-Up), pakaian, noda semen, rintik hujan, dan pencahayaan karakter **100% KONSISTEN TANPA BERUBAH SEDIKIT PUN**!
