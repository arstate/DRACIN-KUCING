# 04. STANDAR PROMPT IMAGE-TO-VIDEO (Img2Vid) & SINKRONISASI DIALOG
## Pedoman Konversi Gambar Diam Menjadi Video Gerak Vertikal (9:16)

---

## 🎬 1. REKOMENDASI MESIN VIDEO AI
Workflow ini dioptimalkan untuk mesin AI video generasi terbaru:
1. **Kling AI 1.6 / 1.5 Pro** (Rekomendasi tertinggi untuk ekspresi wajah feline, gerak fisik alami, dan durasi 5s/10s).
2. **Runway Gen-3 Alpha Turbo** (Sangat bagus untuk dynamic tracking, efek hujan badai, dan lighting dramatis).
3. **Hailuo AI (Minimax Video-01)** (Gerak cakar dan interaksi antar karakter sangat mulus tanpa morphing).
4. **Luma Dream Machine 1.5** (Transisi kamera handheld yang sinematik).

---

## 📂 2. FIRST-FRAME IMAGE INPUT WORKFLOW
* **Kunci Keberhasilan:** Jangan mengenerate video dari teks murni (*Text-to-Video*) karena karakter akan berubah!
* **Wajib Gunakan Gambar Master/Multishot sebagai First Frame (Start Frame):**
  1. Pilih 1 gambar terbaik hasil generate Nano Banana 2.1 dari folder `HASIL_GEN_MASTER/` atau `HASIL_GEN_MULTISHOT/`.
  2. Masukkan file tersebut ke folder `INPUT_REF_VIDEO/` dengan nama: `S1_SCENE_XX_REF_FOR_VIDEO.png`.
  3. Upload gambar tersebut sebagai **Start Frame (First Frame Image)** di dashboard Kling AI / Runway Gen-3.
  4. Tempelkan prompt video operasional.
  5. Simpan file video akhir (.mp4) ke dalam folder: `HASIL_GEN_VIDEO/S1_SCENE_XX_VIDEO.mp4`.

---

## 🎥 3. FORMULA GERAK KAMERA (ORGANIC HANDHELD OPERATOR)
Hindari instruksi gerak kamera kaku seperti drone mekanis atau sliding rel datar. Gunakan deskripsi kamera juru kamera manusia (*shoulder-rig operator*):

* **Kamera Handheld Organik:** `Organic handheld camera with natural subtle operator shoulder-rig micro jitter and gentle breathing sway.`
* **Snap Zoom Emosional:** `Fast dynamic snap zoom-in onto character's shocked feline eyes, freezing at peak impact.`
* **Tracking Mundur/Maju:** `Cinematic handheld camera slowly tracks backward/forward at eye-level, maintaining character in central thirds.`
* **Ground-Level Shudder:** `Ground-level low-angle handheld camera with slight sudden impact shudder as the foot stomps the ground.`

---

## ⏱️ 4. PANDUAN PILIHAN DURASI & SINKRONISASI DIALOG
Untuk mencegah dialog percakapan terpotong sebelum aksi selesai, gunakan panduan durasi per shot/scene berikut:

### 🟡 Opsi 4 Detik (Pacing Super Cepat TikTok / Reels):
* **Karakter:** Aksi kinetik cepat, 1 kalimat dialog pendek (maksimal 6-8 kata).
* **Pola Waktu:**
  * Detik 00:00 - 00:02: Aksi fisik (misal: menjatuhkan sak semen, atau membuka kotak cincin).
  * Detik 00:02 - 00:04: Reaksi wajah + 1 baris dialog singkat menusuk.

### 🟢 Opsi 6 Detik (STANDAR PALING DIREKOMENDASIKAN):
* **Karakter:** Keseimbangan sempurna antara pembentukan emosi, detail gerakan fisik, dan percakapan 2 arah yang utuh.
* **Pola Waktu:**
  * Detik 00:00 - 00:02: Aksi pembuka / interaksi awal karakter.
  * Detik 00:02 - 00:04: Dialog utama dari karakter pertama (misal pertanyaan harga atau lamaran).
  * Detik 00:04 - 00:06: Reaksi balasan karakter kedua (jawaban histeris / tendangan / seringai) + transisi.

### 🔵 Opsi 8 - 10 Detik (Extended Melodrama & Puncak Ending Gantung):
* **Karakter:** Khusus untuk adegan emosional mendalam (patah hati di tengah hujan) atau titik puncak cliffhanger di Scene 4.
* **Pola Waktu:**
  * Detik 00:00 - 00:04: Eksplorasi suasana dramatis (suara hujan badai, langkah gontai, napas lelah).
  * Detik 00:04 - 00:07: Dialog batin atau percakapan telepon berwibawa.
  * Detik 00:07 - 00:10: Klimaks suara keras (petir menggelegar, perintah bekukan aset) -> **HARD CUT TO BLACK**.

---

## 🔊 5. SOUNDSCAPE AUDIO & PANDUAN SFX
Setiap berkas prompt video menyertakan 4 lapisan audio untuk proses editing akhir di CapCut / Premiere:
1. **Lapisan Ambience (Suasana Ruang):** Gemuruh hujan badai, gemercik air selokan, dengung lampu kristal ballroom, desau angin bukit.
2. **Lapisan Foley (Suara Benda Nyata):** Langkah bot basah di kubangan, suara tendangan keras stiletto `DUKKK!`, kaleng seng beradu aspal `KLENGGG!`, koin berhamburan `PYARRR!`, klik kotak cincin `KLIK!`, tuts tombol telepon satelit `BEEP-BEEP`.
3. **Lapisan Voiceover / Dialog:** Suara tulus bergetar Oyen kuli, suara cempreng manja serakah Molly, suara tawa bariton congkak Grevy, dan suara dingin kaisar mutlak Oyen saat bangkit.
4. **Lapisan Musik:** Alunan biola cello melankolis yang tiba-tiba berhenti total saat petir menyambar, menyisakan **HENING TOTAL** di layar hitam CTA.
