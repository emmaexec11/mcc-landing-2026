# MCC Landing Page — Photo Swap List

Every spot in `index.html` that has a placeholder photo. Replace these with real photos when ready (Higgsfield-generated, real customer photos, or iPhone selfies). The code is structured so each swap is a single `src=` URL change — the layout/styling stays the same.

Each placeholder has a `data-replace-photo` attribute in the HTML to make it easy to find with Cmd+F.

---

## 🔴 PRIORITY 1 — FOUNDER PORTRAIT (highest trust impact)

**Where:** Offer card → Founder note (`data-replace-photo="founder-portrait-devon"`)
**Size:** 96px circle (rendered)
**Current placeholder:** `ChatGPT_Image_Jan_12_2026_10_03_14_AM.png` — AI-generated, hurts trust
**Replace with:** Real iPhone selfie of Devon in the Kelowna lab (or anywhere natural)
**Why it matters:** Customers subconsciously detect AI photos. Single biggest UX upgrade on the page. Takes 30 seconds to fix.
**Aspect ratio:** 1:1 square (gets cropped to circle)

---

## 🟡 PRIORITY 2 — EDITORIAL LIFESTYLE HERO

**Where:** "Why We're Not Like Other Makeup" section, circular lifestyle photo (`data-replace-photo="why-different-lifestyle-hero"`)
**Size:** ~460px round (88% of 520px container)
**Current placeholder:** `Multi_Testimonial_1.png` — works but generic testimonial face
**Replace with:** Editorial portrait of a customer applying or wearing MCC
**Style direction:**
- Golden hour or soft daylight
- Natural authentic moment (not posed studio shot)
- Dewy skin, real makeup look
- Aesthetic: Vintner's Daughter / Saie / RMS Beauty
- Higgsfield prompt template (use image-to-image with your tin as ref):
  ```
  Editorial beauty photograph: young Canadian woman, mid-20s, soft natural makeup, dewy skin, applying tinted balm to lips with fingertip, golden hour window light, cream linen surface, holding open 7g aluminum tin of natural cream makeup in the other hand, Vintner's Daughter aesthetic, Hasselblad H6D, Fuji 400H film, soft shadows, photoreal authentic moment
  ```
**Aspect ratio:** 1:1 square (gets cropped to circle)

---

## 🟢 PRIORITY 3 — HERO CUSTOMER AVATAR (Jennifer T.)

**Where:** Hero section, Jennifer T. quote card (`data-replace-photo="customer-avatar-jennifer-t"`)
**Size:** 44px round avatar
**Current placeholder:** `Multi_Testimonial.png` — generic testimonial photo
**Replace with:** Headshot of a real customer (ideally an actual customer named Jennifer if you have one, OR rename the quote to match whoever's headshot you use)
**Style direction:** Natural lighting, smiling, friendly, looks like a real person not a stock photo
**Aspect ratio:** 1:1 square (gets cropped to circle)

---

## ✅ ALREADY REAL — NO SWAP NEEDED

**Hero product image** (`Multi_colour_cream_bundle_sharpened.jpg`) — your real bundle photo, looks great
**Offer card product image** (`Multi_colour_cream_8.png`) — your real 3-tin photo with floating badges
**Desktop sticky CTA thumbnail** — same bundle photo, scaled down
**UGC video #1** (`customer-application.mp4`) — your real photoshoot video, gorgeous
**UGC video #2** (`product-pan.mp4`) — your real macro product video
**UGC videos #3-5** — Shopify CDN customer videos (Shaye, Jamye, Mya)
**Floating customer review photos** — done via initial-circle avatars, looks intentional

---

## OPTIONAL UPGRADES (nice-to-have, not blocking 10/10)

### Ingredient hero photos
Currently the Ingredients section uses emoji icons (🍇🍃💧). Could add 3 real overhead photos:
- Real raspberries on cream linen (for "Real fruit pigments")
- Jojoba + shea butter + green tea flat-lay (for "Skin-loving botanicals")
- Hyaluronic dropper + olive squalane bottle (for "Hydrating support")

Higgsfield prompt for any of these:
```
Overhead photograph: [ingredients] arranged on natural cream linen cloth, soft natural window light from upper left, professional clean-beauty editorial photography, Hasselblad H6D, Fuji Provia 400X film, shallow depth of field, warm cottage-table aesthetic, no people, no text, no product
```

### Behind-the-scenes lab shot
Could add a hand-pouring shot between the "How It Works" and "UGC Reel" sections to back up the "hand-poured this week" claim.

```
Behind-the-scenes photograph: female hands pouring melted natural cream makeup from a small ladle into an open 7g aluminum tin on a wooden workbench, Kelowna BC artisanal beauty lab, soft natural side light, warm cream and forest green palette, no faces visible, editorial documentary photography style
```

---

## HOW TO SWAP A PHOTO

1. Generate or take the real photo
2. Upload to Shopify CDN via your admin (Settings → Files → Upload)
3. Copy the file URL
4. Open `index.html`
5. Cmd+F for `data-replace-photo="[name]"` (e.g. `data-replace-photo="founder-portrait-devon"`)
6. Replace the `src="..."` URL inside that block with your new Shopify CDN URL
7. Commit, push, done

Alternatively, just send the photos to me in chat and I'll swap them in within 5 min.
