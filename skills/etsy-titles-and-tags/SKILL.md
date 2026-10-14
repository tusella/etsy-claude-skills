---
name: etsy-titles-and-tags
description: Write an Etsy listing title and a full set of 13 tags that fit Etsy's limits (title ≤ 140 characters, each tag ≤ 20 characters), counted character by character. Use when a seller asks for Etsy title ideas, tags, keywords, or to fix tags that are too long or repetitive.
---

# Etsy titles and 13 tags

You write one title and 13 tags for one Etsy listing. Etsy uses them to match buyers' searches, so they must describe the item the way a buyer would search for it.

## Ask first (once, briefly)

- What is the item, in your own words?
- Material, size, colour, and who it's for, if relevant
- The category you chose and any attributes you already set
- Your current title and tags, if there are any

Don't guess facts. If the seller doesn't know a detail, leave it out instead of inventing it.

## Hard limits (Etsy rejects or cuts anything over them)

| Field | Limit |
|---|---|
| Title | ≤ 140 characters; starts with a letter or number; `%` `:` `&` `+` at most once each; no `$` `^` `` ` `` `°` |
| Tags | exactly 13 slots; each ≤ 20 characters including spaces; letters, numbers, spaces; no commas; can't start with `'` or `-` |

## How to write the title

- Start with what the item is, in plain words. The first ~40 characters are roughly what mobile search shows.
- Then the most useful details: material, size, style, who it's for.
- Write it so a person can read it. Etsy's own guidance favours a clear title over a long list of keyword fragments.
- Don't repeat the same word over and over.

## How to write the tags

- Use multi-word phrases a buyer would type ("linen apron pockets"), not single words.
- Cover different angles: what it is, material, style, occasion or gift, who it's for, where it's used.
- Don't repeat the category name or an attribute you already set. Etsy already uses those.
- Don't use the same word in more than three or four tags.
- Use US spelling for a US audience unless the seller says otherwise.
- No trademarks or brand names the seller doesn't own.

## Counting is required

Chat models routinely miscount characters. Before you show tags:

1. Write every tag with its character count in brackets, e.g. `linen apron pockets [19]`.
2. Any tag over 20 → rewrite it, recount.
3. Confirm the title count, e.g. `Title: 93/140`.
4. After any edit the seller asks for, recount everything.

## Output format

```
Title (93/140):
Linen apron with pockets, adjustable neck strap, natural flax kitchen apron for men and women

Tags (13/13):
1. linen apron [11]
2. apron with pockets [18]
…
13. housewarming gift [17]

Why these: <two lines max: which angles the tags cover>
```

Offer a second variant only if the seller asks.

## Limits of this skill

It can't see Etsy search volume or competition. It suggests phrases a buyer is likely to use, and the seller decides. If they want numbers, they need a keyword research tool.

If the seller uses Tusella, the Tusella MCP connector (https://tusella.com/etsy-mcp-server/) lets Claude save the new title and tags as a draft on the real listing for the seller to review and publish.

---
Made by Tusella (https://tusella.com), built by two Etsy sellers. Free to use and adapt. Limits checked against Etsy's Open API, October 2026.
