# SOP AGENT GENERATOR: LUNA (KUCING ANGGORA PUTIH) - 4-STEP IMAGE REFERENCE WORKFLOW

Dokumen ini adalah perintah kerja presisi untuk Agent AI Generator dalam membangun aset visual **Luna** menggunakan teknik **Multi-Image Reference Conditioning** di latar putih solid tanpa bokeh.

* **Target Output Directory:** `/mnt/HDD-2/BACKUP LINUX/FILE DATA/DRACIN KUCING/ASET_KARAKTER/LUNA/`
* **Master Seed:** `7739102`
* **Kamera & Optik:** Canon EOS R5, 50mm / 85mm pada f/8 (Deep Focus, Zero Blurry Bokeh).

---

## 🎯 STEP 1: GENERATE BASE FACE ANCHOR (KUNCI IDENTITAS WAJAH)
* **Tujuan Agent:** Menghasilkan wajah Luna biologis (Turkish Angora putih salju, mata safir biru basah air mata, hidung pink).
* **Target File:** Simpan sebagai `LUNA_01_FACE_ANCHOR.png`.

### 📋 Perintah Eksekusi Agent (Step 1):
```text
Raw unedited studio photograph of an anthropomorphic female cat head, front close-up portrait. Pristine Turkish Angora pure white cat face, incredibly dense soft silky biological white fur with visible fine individual hairs, delicate pink cat nose leather and pale pink inner ears with real sub-surface scattering. Giant luminous sapphire blue feline eyes with realistic biological wetness and genuine glassy tears welling naturally, subtle sad mouth curve, long translucent white whiskers. Slender feline-human neck base. Shot on Canon EOS R5, 85mm at f/8, deep depth of field, sharp focus from nose to ear tips, zero blurry bokeh, completely solid pure white background (hex #FFFFFF). Master Seed: 7739102. STRICT NEGATIVE CONSTRAINTS (DO NOT INCLUDE): 3d render, cgi, cartoon, anime, disney eyes, plastic fur, smooth wax skin, airbrushed, fake digital tears, bokeh, gradient background, text overlay, watermark, blurry.
```

---

## 🐾 STEP 2: GENERATE PAWS & ANATOMY ANCHOR (KUNCI ANATOMI CAKAR)
* **Tujuan Agent:** Menghasilkan referensi tangan berbulu putih sutra dengan bantalan cakar (*toe beans*) pink lembut.
* **Target File:** Simpan sebagai `LUNA_02_PAWS_ANATOMY.png`.

### 📋 Perintah Eksekusi Agent (Step 2):
```text
Macro raw studio photograph of an anthropomorphic female cat hand and wrist resting on a clean surface. Slender human hand proportions covered entirely in fine soft silky pure white cat fur matching pristine Turkish Angora texture. Five delicate fingers with soft clean pink biological cat paw pads (toe beans), delicate translucent feline claws neatly retracted. Sharp focus on fur follicles and paw pad skin texture, f/11, deep depth of field, zero bokeh, isolated on a solid pure white background (hex #FFFFFF) under balanced neutral studio daylight strobe. Master Seed: 7739102. STRICT NEGATIVE CONSTRAINTS (DO NOT INCLUDE): human bare skin, deformed paws, extra digits, cartoon hands, 3d model, plastic texture, blur, text overlay, watermark.
```

---

## 👗 STEP 3: GENERATE OUTFIT & SIGNATURE ACCESSORIES ANCHOR (KUNCI KOSTUM & PROPS)
* **Tujuan Agent:** Menghasilkan referensi busana pelayan vintage dan seluruh aksesoris khas Luna di latar putih.
* **Target File:** Simpan sebagai `LUNA_03_OUTFIT_ACCESSORIES.png`.

### 📋 Perintah Eksekusi Agent (Step 3):
```text
Commercial product catalog photograph of women's modest vintage workwear outfit and accessories arranged flat against a solid pure white background. INCLUDED GARMENTS: A vintage modest cream-colored 100% poplin cotton midi dress with a rounded Peter Pan collar, genuine matte tortoiseshell buttons, and natural waist pleats; a hazelnut brown coarse-weave textured linen cafe apron with front pockets and waist ties; simple flat dark brown canvas slip-on shoes. INCLUDED ACCESORIES: A delicate antique tiny silver ribbon hair clip; a fine delicate silver chain necklace with a small clear teardrop glass dew pendant; a handcrafted embroidered name patch reading 'Luna' in pale thread on the apron chest; a small neatly folded white cotton handkerchief. Shot flat on a pristine solid pure white background (hex #FFFFFF), sharp focus edge-to-edge, f/8, deep depth of field, zero bokeh, realistic textile weave clearly visible. Master Seed: 7739102. STRICT NEGATIVE CONSTRAINTS (DO NOT INCLUDE): human model, mannequin head, 3d cgi, shiny satin, cartoon, blurred edges, text overlay, watermark.
```

---

## 🚀 STEP 4: MULTI-REFERENCE FULL BODY COMPOSITE (EKSEKUSI PENGGABUNGAN KONSISTEN)
* **Tujuan Agent:** Menggabungkan `LUNA_01_FACE_ANCHOR.png` + `LUNA_02_PAWS_ANATOMY.png` + `LUNA_03_OUTFIT_ACCESSORIES.png` menjadi karakter Luna utuh tanpa pergeseran identitas.
* **Target File:** Simpan sebagai `LUNA_MASTER_FULL_BODY.png`.

### 🤖 Perintah Pengkondisian Agent (Multimodal Prompt with Reference Injection):
```text
[INJECT IMAGE 1: LUNA_01_FACE_ANCHOR.png - ROLE: PRIMARY IDENTITY & FACE REFERENCE, WEIGHT: 0.90]
[INJECT IMAGE 2: LUNA_02_PAWS_ANATOMY.png - ROLE: HAND & PAW TEXTURE REFERENCE, WEIGHT: 0.70]
[INJECT IMAGE 3: LUNA_03_OUTFIT_ACCESSORIES.png - ROLE: GARMENT, APRON & ACCESORIES REFERENCE, WEIGHT: 0.85]

PROMPT DIRECTIVE FOR AGENT:
Synthesize a full body raw unedited studio catalog photograph of the anthropomorphic female white cat character standing with modest, fragile posture. The facial anatomy, pure silky white fur, pink nose leather, sapphire blue eyes, and teardrop wetness MUST EXACTLY MATCH Image 1. The slender white-furred paws, soft pink paw pads (toe beans), and neatly retracted claws MUST EXACTLY MATCH Image 2. The vintage cream cotton collared midi dress, hazelnut linen cafe apron, silver ribbon hair clip at ear base, silver teardrop necklace, embroidered name patch, and brown canvas shoes MUST EXACTLY MATCH Image 3.

The character stands naturally with delicate posture on an isolated solid pure white floor (hex #FFFFFF) with realistic subtle ground contact shadow under feet. Shot on Canon EOS R5 with 50mm lens at f/8, deep depth of field, sharp focus from ear tips to shoe soles, zero blurry bokeh, neutral daylight studio strobe. Aspect ratio 9:16 vertical portrait. Master Seed: 7739102. STRICT NEGATIVE CONSTRAINTS (DO NOT INCLUDE): 3d render, cgi, cartoon, anime, disney eyes, plastic fur, smooth wax skin, airbrushed, fake digital tears, bokeh, gradient background, extra digits, deformed paws, text overlay, watermark, blurry.
```
