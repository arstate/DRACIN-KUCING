# SOP AGENT GENERATOR: CLEO (SIAMESE ROYAL SOCIALITE) - 4-STEP IMAGE REFERENCE WORKFLOW

Dokumen ini adalah perintah kerja presisi untuk Agent AI Generator dalam membangun aset visual **Cleo** menggunakan teknik **Multi-Image Reference Conditioning** di latar putih solid tanpa bokeh.

* **Target Output Directory:** `/mnt/HDD-2/BACKUP LINUX/FILE DATA/DRACIN KUCING/ASET_KARAKTER/CLEO/`
* **Master Seed:** `5517104`
* **Kamera & Optik:** Canon EOS R5, 50mm / 85mm pada f/8 (Deep Focus, Zero Blurry Bokeh).

---

## 🎯 STEP 1: GENERATE BASE FACE ANCHOR (KUNCI IDENTITAS WAJAH)
* **Tujuan Agent:** Menghasilkan wajah kucing Siam elegan culas dengan gradasi cokelat seal-point dan mata biru kobalt.
* **Target File:** Simpan sebagai `CLEO_01_FACE_ANCHOR.png`.

### 📋 Perintah Eksekusi Agent (Step 1):
```text
Raw unedited studio photograph of an anthropomorphic female cat head, front close-up portrait. Exquisite Siamese royal cat face, striking chocolate seal-point facial mask gradient fading into creamy beige neck fur. Piercing cold almond-shaped cobalt blue feline eyes with arched dismissive brow, dark chocolate nose leather, subtle arrogant smirk on lips, fine dark whiskers. Slender feline-human neck base. Shot on Canon EOS R5, 85mm at f/8, deep depth of field, sharp focus across entire face from ear tips to jawline, zero blurry bokeh, completely solid pure white background (hex #FFFFFF). Master Seed: 5517104. STRICT NEGATIVE CONSTRAINTS (DO NOT INCLUDE): cartoon, 3d model, anime, cgi, illustration, plastic texture, wax face, blurry, gradient background, deformed ears, text overlay, watermark.
```

---

## 🐾 STEP 2: GENERATE PAWS & ANATOMY ANCHOR (KUNCI ANATOMI CAKAR & MANICURE)
* **Tujuan Agent:** Menghasilkan referensi tangan berbulu cokelat Siam dengan cakar lentik berkuteks merah mengkilap.
* **Target File:** Simpan sebagai `CLEO_02_PAWS_ANATOMY.png`.

### 📋 Perintah Eksekusi Agent (Step 2):
```text
Macro raw studio photograph of an anthropomorphic female cat hand and wrist posing with haughty grace on a clean surface. Slender human female hand proportions covered in short, dense dark chocolate-brown feline fur. Five delicate fingers featuring soft dark brown biological cat paw pads (toe beans) and sharp manicured feline claws finished in glossy high-shine scarlet crimson red nail polish. Sharp focus on fur follicles, claw curvature, and lacquer shine, f/11, deep depth of field, zero bokeh, isolated on a solid pure white background (hex #FFFFFF) under neutral studio daylight strobe. Master Seed: 5517104. STRICT NEGATIVE CONSTRAINTS (DO NOT INCLUDE): human bare skin, deformed paws, chipped polish, cartoon hands, 3d model, plastic texture, blur, text overlay, watermark.
```

---

## 👗 STEP 3: GENERATE OUTFIT & SIGNATURE ACCESSORIES ANCHOR (KUNCI KOSTUM & PROPS)
* **Tujuan Agent:** Menghasilkan referensi gaun satin merah desainer dan seluruh perhiasan mewah Cleo di latar putih.
* **Target File:** Simpan sebagai `CLEO_03_OUTFIT_ACCESSORIES.png`.

### 📋 Perintah Eksekusi Agent (Step 3):
```text
Commercial product catalog photograph of women's haute couture eveningwear and luxury diamond jewelry arranged flat against a solid pure white background. INCLUDED GARMENTS: A floor-length off-shoulder scarlet crimson silk satin mermaid gown with draped hip pleats and a structured corset bodice; an authentic thick genuine white fox fur stole; scarlet red satin pointed-toe stiletto high heels. INCLUDED ACCESORIES: Vintage cat-eye sunglasses with crystal-studded gold frames; a lavish four-strand genuine white freshwater pearl choker necklace; sparkling platinum diamond chandelier drop earrings; a white gold tennis bracelet encrusted with royal blue sapphires; a miniature structured crimson crocodile-embossed leather designer clutch bag with gold lock. Shot flat on a pristine solid pure white background (hex #FFFFFF), sharp focus edge-to-edge, f/8, deep depth of field, zero bokeh, lustrous satin sheen and gemstone refraction clearly visible. Master Seed: 5517104. STRICT NEGATIVE CONSTRAINTS (DO NOT INCLUDE): mannequin head, human body, 3d cgi, cheap fabric, cartoon, blurred edges, text overlay, watermark.
```

---

## 🚀 STEP 4: MULTI-REFERENCE FULL BODY COMPOSITE (EKSEKUSI PENGGABUNGAN KONSISTEN)
* **Tujuan Agent:** Menggabungkan `CLEO_01_FACE_ANCHOR.png` + `CLEO_02_PAWS_ANATOMY.png` + `CLEO_03_OUTFIT_ACCESSORIES.png` menjadi karakter Cleo utuh tanpa pergeseran identitas.
* **Target File:** Simpan sebagai `CLEO_MASTER_FULL_BODY.png`.

### 🤖 Perintah Pengkondisian Agent (Multimodal Prompt with Reference Injection):
```text
[INJECT IMAGE 1: CLEO_01_FACE_ANCHOR.png - ROLE: PRIMARY IDENTITY & FACE REFERENCE, WEIGHT: 0.90]
[INJECT IMAGE 2: CLEO_02_PAWS_ANATOMY.png - ROLE: HAND & MANICURED CLAW REFERENCE, WEIGHT: 0.70]
[INJECT IMAGE 3: CLEO_03_OUTFIT_ACCESSORIES.png - ROLE: GOWN, FUR STOLE & JEWELRY REFERENCE, WEIGHT: 0.85]

PROMPT DIRECTIVE FOR AGENT:
Synthesize a full body raw unedited studio catalog photograph of the anthropomorphic female Siamese cat character standing with haughty, malicious elegance. The facial anatomy, chocolate seal-point gradient mask, creamy neck, cobalt blue eyes, and dismissive brow MUST EXACTLY MATCH Image 1. The chocolate fur paws with glossy crimson red manicured claws MUST EXACTLY MATCH Image 2. The scarlet crimson silk satin mermaid gown, white fox fur stole, crystal cat-eye sunglasses on forehead, pearl choker, diamond chandelier earrings, sapphire bracelet, red crocodile clutch bag, and red stiletto heels MUST EXACTLY MATCH Image 3.

The character stands with elegant hourglass posture on an isolated solid pure white floor (hex #FFFFFF) with clean subtle contact shadow. Shot on Canon EOS R5 with 50mm lens at f/8, deep depth of field, sharp focus from ear tips to stiletto heels, zero blurry bokeh, neutral balanced high-fashion studio strobe. Aspect ratio 9:16 vertical portrait. Master Seed: 5517104. STRICT NEGATIVE CONSTRAINTS (DO NOT INCLUDE): cartoon, 3d model, anime, cgi, illustration, plastic texture, wax face, blurry, bad hands, deformed paws, text overlay, watermark.
```
