---
name: etsy-main-photo-check
description: Check whether an Etsy listing's main photo survives Etsy's different crops (square in search, taller on mobile, wider in emails and ads) and review the photo set for gaps. Use when a seller shares an Etsy product photo or asks about thumbnails, cropping, photo order, or which photos a listing is missing.
---

# Etsy main photo check

Etsy uses the first photo of a listing in several places and crops it differently in each. A product that looks fine in one place can lose its edges in another. You check that, and you check the photo set for obvious gaps.

## The crop geometry

Etsy shows the main photo:

- **square (1:1)** in search results
- **taller (about 4:5)** on mobile, which cuts the sides
- **wider (about 4:3)** in emails, Offsite Ads and "you may also like" rows, which cuts the top and bottom

These ratios are measured approximations; Etsy doesn't publish exact numbers. The area that survives every crop is roughly the **central 80% of the width × 75% of the height** of a square photo. The product must sit fully inside it.

## How to check an image

If you can see the image:

1. Estimate the product's bounding box as a share of the frame (left, right, top, bottom margins in %).
2. Compare with the safe zone: at least ~10% margin on each side, ~12.5% at the top and bottom.
3. Report plainly: "Left edge of the bowl is ~4% from the frame edge, so the mobile crop will cut it."
4. Check that the photo is square or close to it. A very wide or tall original gets cropped hard.
5. Check that the product fills a good part of the safe zone. A tiny product in the middle is safe but hard to see at thumbnail size.

Composition note: rule-of-thirds placement looks good in lifestyle photos but gets cropped in the main photo. For the first photo, centre the product and let it fill most of the safe zone.

If you can't see the image, explain the rule and ask for a description or the image.

## Photo set review (facts only)

If the seller lists all photos, report:

- count out of 20 (Etsy allows up to 20; some help pages still say 10)
- whether there's a video (5–15 seconds; Etsy removes the sound)
- whether there's a scale shot (in hand, on a person, next to a common object)
- whether there's a detail or texture shot
- whether variations (colours, sizes) are each shown
- transparent PNGs: Etsy shows transparency as black, so flatten onto a background
- alt text present or not (≤ 500 characters)

Don't give a score. List what's there, what's missing, and one concrete next shot to take.

## Output

```
Main photo
- Ratio: 3:2 (wide), so search will crop the sides hard
- Product margins: L 4% · R 6% · T 18% · B 15%
- Mobile crop (sides): cuts the left edge of the product
- Fix: re-crop to square, product centred, ~10% clear on each side

Photo set: 6/20 · video: no · scale shot: no · detail shot: yes
Next shot to take: the bag on a shoulder, for scale
```

## With Tusella

Tusella's photo editor has an Etsy-safe crop preset that shows these zones and frames the product automatically: https://tusella.com

---
Made by Tusella (https://tusella.com), built by two Etsy sellers. Free to use and adapt. October 2026.
