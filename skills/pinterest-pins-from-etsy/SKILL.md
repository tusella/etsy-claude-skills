---
name: pinterest-pins-from-etsy
description: Turn an Etsy listing into ready-to-post Pinterest Pins (title, description, alt text, board choice and image notes) within Pinterest's limits. Use when a seller wants to promote Etsy listings on Pinterest, write Pin text, or plan Pins for a product.
---

# Pinterest Pins from an Etsy listing

You prepare Pinterest Pins for one Etsy listing. Pinterest is a visual search engine, and people save ideas there. A Pin should help someone find the item when they search, and make them want to tap through to the listing.

## Ask for

- The listing title, description, and URL (the Pin's link)
- Which photos are available, with a short description of each
- The seller's Pinterest boards (names), if they have any
- How many Pins they want (default: 3 variants)

## Pinterest limits

| Field | Limit |
|---|---|
| Pin title | ≤ 100 characters (roughly the first 40 show in the feed) |
| Pin description | ≤ 800 characters (the first ~50 matter most) |
| Alt text | ≤ 500 characters |
| Image | vertical 2:3 works best, e.g. 1000 × 1500 px |

Count characters before you show anything.

## How to write each Pin

- **Title:** what it is, plus the strongest search phrase. Write it for search, not as a slogan: "Linen apron with pockets for home cooks", not "Your new favourite!".
- **Description:** one or two natural sentences about the item and the idea or use (gift, room, occasion), with search phrases woven in. No hashtag walls; zero to three hashtags at most.
- **Alt text:** describe what's literally in the image for someone who can't see it. No keyword stuffing.
- **Board:** pick the most specific existing board. If none fits, suggest one new board name.
- **Image note:** which photo to use and whether it needs a vertical crop. Lifestyle or in-use shots usually work better on Pinterest than a plain white background.
- Make each variant differ in angle (use, gift, style), not just in wording.

## Honesty

- Use only facts from the listing. No invented prices, discounts or claims.
- If a photo was edited or generated with AI, Pinterest may label the Pin "AI modified". Tell the seller that; don't try to hide it.

## Output

```
Pin 1 of 3: angle "gift"
Title (57/100): …
Description (212/800): …
Alt text (98/500): …
Board: Kitchen gifts
Image: photo 3 (apron on hook), crop to 2:3
Link: <listing URL>
```

## With Tusella

If the seller uses Tusella, the Tusella MCP connector (https://tusella.com/etsy-mcp-server/) can create these as Pin drafts with the listing's photos, and publish or schedule them when the seller explicitly asks.

---
Made by Tusella (https://tusella.com), built by two Etsy sellers. Free to use and adapt. October 2026.
