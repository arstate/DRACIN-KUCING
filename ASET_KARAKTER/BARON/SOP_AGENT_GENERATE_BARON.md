# SOP AGENT GENERATOR: BARON (BENGAL LEOPARD TYCOON) - 4-STEP IMAGE REFERENCE WORKFLOW

Dokumen ini adalah perintah kerja presisi untuk Agent AI Generator dalam membangun aset visual **Baron** menggunakan teknik **Multi-Image Reference Conditioning** di latar putih solid tanpa bokeh.

* **Target Output Directory:** `/mnt/HDD-2/BACKUP LINUX/FILE DATA/DRACIN KUCING/ASET_KARAKTER/BARON/`
* **Master Seed:** `6628103`
* **Kamera & Optik:** Canon EOS R5, 50mm / 85mm pada f/8 (Deep Focus, Zero Blurry Bokeh).

---

## 🎯 STEP 1: GENERATE BASE FACE ANCHOR (KUNCI IDENTITAS WAJAH)
* **Tujuan Agent:** Menghasilkan wajah Bengal Leopard berwibawa bengis dengan bintik roset tajam dan mata hijau es.
* **Target File:** Simpan sebagai `BARON_01_FACE_ANCHOR.png`.

### 📋 Perintah Eksekusi Agent (Step 1):
```text
Raw unedited studio photograph of an anthropomorphic male cat head, front close-up portrait. Imposing Bengal leopard cat face, sleek golden-tawny fur with authentic bold dark leopard rosettes and distinct forehead facial striping. Biologically accurate predatory feline features, dark leather nose, piercing icy pale green feline eyes with sharp vertical slits, subtle arrogant cruel smirk, fine stiff whiskers. Muscular human-feline neck base. Shot on Canon EOS R5, 85mm at f/8, deep depth of field, sharp focus across entire face from ear tips to whiskers, zero blurry bokeh, completely solid pure white background (hex #FFFFFF). Master Seed: 6628103. STRICT NEGATIVE CONSTRAINTS (DO NOT INCLUDE): cartoon, 3d render, anime, cgi, illustration, plastic skin, wax figure, domestic cat fur, round pupils, blurry, gradient background, text overlay, watermark.
```

---

## 🐾 STEP 2: GENERATE PAWS & ANATOMY ANCHOR (KUNCI ANATOMI CAKAR)
* **Tujuan Agent:** Menghasilkan referensi tangan berbulu tutul Bengal dengan cakar tajam dan bantalan cakar gelap.
* **Target File:** Simpan sebagai `BARON_02_PAWS_ANATOMY.png`.

### 📋 Perintah Eksekusi Agent (Step 2):
```text
Macro raw studio photograph of an anthropomorphic male cat hand and wrist resting flat on a white surface. Strong masculine human hand anatomy covered in sleek short golden-tawny fur with distinct leopard rosettes. Five fingers featuring tough dark charcoal biological cat paw pads (toe beans) and sharp, semi-retracted curved feline claws. Veins and muscular knuckles subtly defined under the pelt. Deep depth of field, f/11 aperture, perfectly sharp focus on claws and skin texture, zero bokeh, isolated on a solid pure white background (hex #FFFFFF) under neutral balanced studio strobe. Master Seed: 6628103. STRICT NEGATIVE CONSTRAINTS (DO NOT INCLUDE): human naked hand, extra fingers, cartoon paws, 3d model, plastic texture, fake cgi, blurry edges, text overlay, watermark.
```

---

## 👔 STEP 3: GENERATE OUTFIT & SIGNATURE ACCESSORIES ANCHOR (KUNCI KOSTUM & PROPS)
* **Tujuan Agent:** Menghasilkan referensi setelan jas wol pinstripe bespoke dan seluruh aksesoris mewah Baron di latar putih.
* **Target File:** Simpan sebagai `BARON_03_OUTFIT_ACCESSORIES.png`.

### 📋 Perintah Eksekusi Agent (Step 3):
```text
Commercial product catalog photograph of men's ultra-luxury three-piece tailored bespoke suit and antique accessories arranged flat against a solid pure white background. INCLUDED GARMENTS: A bespoke three-piece charcoal pinstripe tailored suit made of heavy English wool with black silk peak lapels, matching pinstripe vest, crisp white dress shirt with French cuffs, deep maroon silk necktie with ruby tie pin, and polished black Italian leather oxford shoes. INCLUDED ACCESORIES: An authentic solid ebony walking cane with an ornate heavy solid silver wolf head handle; an antique solid gold pocket watch with heavy chain; a frameless gold-rimmed reading monocle attached to a fine gold ear-chain; a heavy solid gold signet ring engraved with a coiled serpent emblem set with a tiny ruby. Shot flat on a pristine solid pure white background (hex #FFFFFF), sharp focus edge-to-edge, f/8, deep depth of field, zero bokeh, textile weave and silver metal sheen clearly visible. Master Seed: 6628103. STRICT NEGATIVE CONSTRAINTS (DO NOT INCLUDE): mannequin head, human body, 3d cgi, cheap polyester, cartoon, blurred edges, text overlay, watermark.
```

---

## 🚀 STEP 4: MULTI-REFERENCE FULL BODY COMPOSITE (EKSEKUSI PENGGABUNGAN KONSISTEN)
* **Tujuan Agent:** Menggabungkan `BARON_01_FACE_ANCHOR.png` + `BARON_02_PAWS_ANATOMY.png` + `BARON_03_OUTFIT_ACCESSORIES.png` menjadi karakter Baron utuh tanpa pergeseran identitas.
* **Target File:** Simpan sebagai `BARON_MASTER_FULL_BODY.png`.

### 🤖 Perintah Pengkondisian Agent (Multimodal Prompt with Reference Injection):
```text
[INJECT IMAGE 1: BARON_01_FACE_ANCHOR.png - ROLE: PRIMARY IDENTITY & FACE REFERENCE, WEIGHT: 0.90]
[INJECT IMAGE 2: BARON_02_PAWS_ANATOMY.png - ROLE: HAND & PAW TEXTURE REFERENCE, WEIGHT: 0.70]
[INJECT IMAGE 3: BARON_03_OUTFIT_ACCESSORIES.png - ROLE: GARMENT, SUIT, CANE & ACCESORIES REFERENCE, WEIGHT: 0.85]

PROMPT DIRECTIVE FOR AGENT:
Synthesize a full body raw unedited studio catalog photograph of the anthropomorphic male Bengal cat character standing with ruthless commanding posture. The facial anatomy, golden-tawny fur with leopard rosettes, icy pale green eyes, and cruel smirk MUST EXACTLY MATCH Image 1. The spotted feline paws, dark paw pads, and sharp claws MUST EXACTLY MATCH Image 2. The bespoke three-piece charcoal pinstripe wool suit, maroon silk tie, ebony cane with silver wolf handle in hand, gold monocle on eye, gold pocket watch chain on vest, gold serpent ring, and polished black oxfords MUST EXACTLY MATCH Image 3.

The character stands tall with imposing dominance on an isolated solid pure white floor (hex #FFFFFF) with sharp subtle floor contact shadow. Shot on Canon EOS R5 with 50mm lens at f/8, deep depth of field, sharp focus from ear tips to shoe soles, zero blurry bokeh, neutral balanced studio lighting. Aspect ratio 9:16 vertical portrait. Master Seed: 6628103. STRICT NEGATIVE CONSTRAINTS (DO NOT INCLUDE): cartoon, 3d render, anime, cgi, illustration, plastic skin, cheap fabric, bad paws, deformed fingers, blurry, gradient background, text overlay, watermark.
```
