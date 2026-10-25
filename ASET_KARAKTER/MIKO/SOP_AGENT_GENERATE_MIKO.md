# SOP AGENT GENERATOR: MIKO (KUCING COWOK OREN) - 4-STEP IMAGE REFERENCE WORKFLOW

Dokumen ini adalah perintah kerja presisi untuk Agent AI Generator dalam membangun aset visual **Miko** menggunakan teknik **Multi-Image Reference Conditioning** di latar putih solid tanpa bokeh.

* **Target Output Directory:** `/mnt/HDD-2/BACKUP LINUX/FILE DATA/DRACIN KUCING/ASET_KARAKTER/MIKO/`
* **Master Seed:** `8849201`
* **Kamera & Optik:** Canon EOS R5, 50mm / 85mm pada f/8 (Deep Focus, Zero Blurry Bokeh).

---

## 🎯 STEP 1: GENERATE BASE FACE ANCHOR (KUNCI IDENTITAS WAJAH)
* **Tujuan Agent:** Menghasilkan wajah Miko biologis dengan tekstur bulu oren, mata tembaga, dan bekas luka telinga kiri.
* **Target File:** Simpan sebagai `MIKO_01_FACE_ANCHOR.png`.

### 📋 Perintah Eksekusi Agent (Step 1):
```text
Raw unedited studio photograph of an anthropomorphic male ginger cat head, front-facing close-up. Authentic domestic orange tabby cat face, genuine coarse warm ginger fur with irregular natural marmalade stripes, white fur patch on chin. Biologically realistic feline features, real moist pinkish cat nose leather with subtle tactile bumps, copper-amber cat eyes with natural vertical pupils and genuine wet specular reflections, fine individual white whiskers sprouting naturally from dark whisker dots, small realistic nick scar on tip of left pointed ear. Human neck base. Shot on Canon EOS R5 with 85mm lens at f/8, deep depth of field, sharp focus across entire face, zero blurry bokeh, completely flat solid pure white background (hex #FFFFFF). Master Seed: 8849201. STRICT NEGATIVE CONSTRAINTS (DO NOT INCLUDE): grey fur, 3d render, cgi, cartoon, pixar, anime, illustration, doll eyes, smooth plastic skin, wax texture, airbrushed fur, digital painting, fake blur, bokeh, shadows on wall, gradient background, text overlay, watermark, blurry.
```

---

## 🐾 STEP 2: GENERATE PAWS & ANATOMY ANCHOR (KUNCI ANATOMI CAKAR)
* **Tujuan Agent:** Menghasilkan referensi tangan berbulu oren dengan bantalan cakar (*toe beans*) dan cakar tumpul nyata.
* **Kondisi:** Pastikan tone warna bulu oren identik dengan `MIKO_01_FACE_ANCHOR.png`.
* **Target File:** Simpan sebagai `MIKO_02_PAWS_ANATOMY.png`.

### 📋 Perintah Eksekusi Agent (Step 2):
```text
Macro raw unedited studio photograph of an anthropomorphic male cat hand and forearm resting flat on a white surface. Realistic human hand anatomy covered in dense natural short ginger-orange feline fur matching warm marmalade tones. Five distinct fingers featuring soft pinkish-grey biological cat paw pads (toe beans) with natural skin creases, equipped with real blunt feline claws extending naturally from nail beds. Veins and knuckles subtly visible under the fur coat. Deep depth of field, f/11 aperture, perfectly sharp focus on every paw pad and claw tip, zero bokeh, shot against an isolated solid pure white background (hex #FFFFFF) under neutral even studio lighting. Master Seed: 8849201. STRICT NEGATIVE CONSTRAINTS (DO NOT INCLUDE): human naked hand, extra fingers, cartoon paws, 3d model, plastic texture, fake cgi, smooth airbrushed skin, blurry edges, watermark, text overlay.
```

---

## 👕 STEP 3: GENERATE OUTFIT & SIGNATURE ACCESSORIES ANCHOR (KUNCI KOSTUM & PROPS)
* **Tujuan Agent:** Menghasilkan referensi pakaian dan seluruh aksesoris Miko yang terisolasi di latar putih.
* **Target File:** Simpan sebagai `MIKO_03_OUTFIT_ACCESSORIES.png`.

### 📋 Perintah Eksekusi Agent (Step 3):
```text
Commercial product catalog photograph of men's complete rugged outfit and accessories cleanly arranged flat against a solid pure white background. INCLUDED GARMENTS: A heavily washed vintage faded blue denim trucker jacket made of genuine 14oz coarse twill cotton with puckered seams and worn brass buttons; a relaxed-fit plain washed black 24s combed cotton crewneck t-shirt with natural cloth folds; dark charcoal ripstop cotton cargo pants with functional side pockets; worn scuffed dark brown leather combat boots. INCLUDED ACCESORIES: An antique heavy oxidized gold medallion pendant carved with a four-fanged lion crest on a tarnished silver chain; a pair of distressed black synthetic leather fingerless riding gloves; a vintage matte black digital wristwatch with a scratched rubber strap; a silver metal motorcycle key ring. Shot flat on a pristine solid pure white background (hex #FFFFFF), sharp focus edge-to-edge, f/8 aperture, zero bokeh, realistic textile weave and metal textures clearly visible. Master Seed: 8849201. STRICT NEGATIVE CONSTRAINTS (DO NOT INCLUDE): mannequin head, human body, 3d render, cartoon, shiny polyester, cgi, blur, text overlay, watermark.
```

---

## 🚀 STEP 4: MULTI-REFERENCE FULL BODY COMPOSITE (EKSEKUSI PENGGABUNGAN KONSISTEN)
* **Tujuan Agent:** Menggabungkan `MIKO_01_FACE_ANCHOR.png` + `MIKO_02_PAWS_ANATOMY.png` + `MIKO_03_OUTFIT_ACCESSORIES.png` menjadi karakter Miko utuh tanpa pergeseran identitas.
* **Target File:** Simpan sebagai `MIKO_MASTER_FULL_BODY.png`.

### 🤖 Perintah Pengkondisian Agent (Multimodal Prompt with Reference Injection):
```text
[INJECT IMAGE 1: MIKO_01_FACE_ANCHOR.png - ROLE: PRIMARY IDENTITY & FACE REFERENCE, WEIGHT: 0.90]
[INJECT IMAGE 2: MIKO_02_PAWS_ANATOMY.png - ROLE: HAND & PAW TEXTURE REFERENCE, WEIGHT: 0.70]
[INJECT IMAGE 3: MIKO_03_OUTFIT_ACCESSORIES.png - ROLE: GARMENT, BOOTS & ACCESORIES REFERENCE, WEIGHT: 0.85]

PROMPT DIRECTIVE FOR AGENT:
Synthesize a full body raw unedited studio catalog photograph of the anthropomorphic male ginger cat character. The facial anatomy, fur color, marmalade stripes, ear scar, and copper-amber eye structure MUST EXACTLY MATCH Image 1. The short ginger-furred hands, paw pads (toe beans), and blunt claws MUST EXACTLY MATCH Image 2. The faded blue denim trucker jacket, black t-shirt, dark charcoal cargo pants, scuffed brown boots, Four-Fanged Lion gold pendant on chest, fingerless gloves, matte black digital watch, and motorcycle keys MUST EXACTLY MATCH Image 3. 

The character stands naturally with confident athletic posture on an isolated solid pure white floor (hex #FFFFFF) with subtle natural contact shadow only. Shot on Canon EOS R5 with 50mm lens at f/8, deep depth of field, sharp focus from ear tips to boot soles, zero blurry bokeh, neutral balanced daylight studio strobe. Aspect ratio 9:16 vertical portrait. Master Seed: 8849201. STRICT NEGATIVE CONSTRAINTS (DO NOT INCLUDE): grey fur, 3d render, cgi, cartoon, anime, illustration, doll eyes, smooth plastic skin, wax texture, airbrushed fur, digital painting, fake blur, bokeh, shadows on wall, gradient background, extra limbs, bad paws, deformed hands, text overlay, watermark, blurry.
```
