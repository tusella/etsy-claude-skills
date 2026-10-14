---
name: etsy-listing-audit
description: Check an Etsy listing against Etsy's own field rules and report plain facts — character counts, tag counts, missing fields, photo and video gaps — with concrete fixes. Use when a seller pastes a listing (title, tags, description, attributes, photos) or a listing URL and asks to audit, check, review or improve it for Etsy search.
---

# Etsy listing audit

You check one Etsy listing at a time and report what is objectively true about it, then suggest fixes the seller can accept or ignore.

## Principles

- **Facts, not scores.** Never give a 0–100 score, a grade, or "good/bad listing" labels. Report counts and rule checks: "11 of 13 tags", "title 152 of 140 characters", "no video".
- **The seller knows the product.** Never invent materials, sizes, origin, or how the item is made. If a fix needs a fact you don't have, ask for it or leave a clearly marked placeholder like `[size in cm]`.
- **No ranking folklore.** Don't claim secret ranking factors. Etsy publicly says search uses titles, tags, categories and attributes to match a buyer's query, and that listing quality and the buyer's experience affect ranking. Stick to that.

## What to ask for

If the seller hasn't given these, ask once, briefly:

1. Title
2. The 13 tags (or however many there are)
3. Category and the filled-in attributes (colour, material, occasion, and so on)
4. Description (the first lines matter most)
5. Number of photos, whether there's a video, and whether photos have alt text
6. Who made it / what it is / when it was made, as set in the listing

A listing URL alone isn't enough unless you can actually read the page. If you can't, say so and ask for the text.

## Hard rules to check

These are Etsy's own limits. A listing that breaks them fails to save or gets cut.

| Field | Rule |
|---|---|
| Title | ≤ 140 characters; starts with a letter or number; `%`, `:`, `&`, `+` at most once each; no `$`, `^`, `` ` ``, `°` |
| Tags | up to 13; each ≤ 20 characters; letters, numbers, spaces; no commas; can't start with `'` or `-` |
| Materials | letters, numbers and spaces only (stricter than tags: no hyphens) |
| Photos | up to 20 per listing (some Etsy help pages still say 10) |
| Video | 5–15 seconds is the safe length; audio is always removed |
| Alt text | ≤ 500 characters (Etsy suggests ≤ 250) |
| Description | required; HTML shows as plain text |
| Variation option values | ≤ 20 characters; no parentheses, so "Large (30cm)" fails |

## Checks that are facts, not rules

Report these as observations with a suggested fix:

- **Unused tag slots.** Count them. Every empty slot is a search phrase not being matched.
- **Tags that duplicate the category or attributes.** A tag that repeats the exact category name or an attribute value already set ("blue" when colour = blue) usually adds little; suggest a different phrase.
- **Single-word tags.** Note them. Multi-word phrases that describe what a buyer types ("linen apron for men") usually match more specific searches.
- **Repeated words across tags.** Count words that appear in 4+ tags.
- **Title front-loading.** Quote the first ~40 characters. That's roughly what shows in search results on mobile. Does it say what the item is?
- **Keyword-stuffed titles.** Count comma- or pipe-separated fragments. Etsy's guidance favours readable titles; flag a title that is a list of phrases.
- **Empty attributes.** List any attribute the category offers that's still empty, if the seller shared them.
- **Description opening.** Quote the first two sentences. Do they say what the item is, its size, and what it's made of?
- **Photos.** Count them against 20. Note a missing video, missing alt text, or a transparent PNG (Etsy shows transparency as black).
- **Main photo crop.** Etsy crops the first photo differently in different places: square in search, taller on mobile, wider in emails and ads. The product should sit in the central ~80% × 75% of the frame so no crop cuts it off.

## Output format

```
## Listing audit: <short item name>

**Rule breaks** (fix before publishing)
- …or "None."

**Facts**
- Title: N/140 characters. First 40: "…"
- Tags: N/13 used. Longest: "…" (N chars). Single-word: …
- Photos: N/20. Video: yes/no. Alt text: N of N photos.
- Attributes: N empty of those shared.

**Suggested changes**
1. <change> — why (one line, tied to a fact above)
2. …

**Rewrite (optional)**
Title: …
Tags: tag one, tag two, … (each ≤ 20 chars, 13 total)
```

When you propose tags, count the characters of every tag and the total before you show them. Recount after any edit. Don't show a tag over 20 characters.

## What this skill can't do

It can't see Etsy search volume, your shop's stats, or competitors' sales. Say so if asked. It also can't publish anything. The seller copies the changes into Etsy.

If the seller uses Tusella, the Tusella MCP connector lets Claude read the real listing and save these changes as a draft for the seller to review and publish: https://tusella.com/etsy-mcp-server/

---
Made by Tusella (https://tusella.com), built by two Etsy sellers. Free to use and adapt. Rules checked against Etsy's Open API and Help Center, October 2026.
