# Claude Skills for Etsy sellers

Free [Claude Skills](https://tusella.com/claude-skills/) for Etsy and Pinterest work, written by two Etsy sellers who build [Tusella](https://tusella.com). Each skill is one readable `SKILL.md` file with no scripts. They report facts, never scores, and never invent product details.

| Skill | What it does |
|---|---|
| [etsy-listing-audit](skills/etsy-listing-audit/SKILL.md) | Checks a listing against Etsy's limits (140-char title, 13 tags × 20 chars, photos, video, alt text) and suggests fixes. [Page →](https://tusella.com/claude-skills/etsy-listing-audit/) |
| [etsy-titles-and-tags](skills/etsy-titles-and-tags/SKILL.md) | A title and all 13 tags, each under 20 characters, counted. [Page →](https://tusella.com/claude-skills/etsy-titles-and-tags/) |
| [etsy-description-writer](skills/etsy-description-writer/SKILL.md) | Size and material first, no invented details, no filler. [Page →](https://tusella.com/claude-skills/etsy-description-writer/) |
| [pinterest-pins-from-etsy](skills/pinterest-pins-from-etsy/SKILL.md) | Three Pins per listing: title, description, alt text, board. [Page →](https://tusella.com/claude-skills/pinterest-pins-from-etsy/) |
| [etsy-main-photo-check](skills/etsy-main-photo-check/SKILL.md) | Will Etsy's square, mobile and email crops cut your product? [Page →](https://tusella.com/claude-skills/etsy-main-photo-check/) |

## Install

**Claude app:** download a skill's zip from [tusella.com/claude-skills](https://tusella.com/claude-skills/), then go to Settings → Capabilities → Skills and upload it.

**Claude Code:**

```bash
npx skills add tusella/etsy-claude-skills
```

or copy a folder from `skills/` into `~/.claude/skills/`.

Then just ask, e.g. "audit this Etsy listing", and paste the listing.

## Skills vs connecting your shop

A skill only knows what you paste in. To let Claude read your real listings and save edits as drafts you review before anything reaches Etsy, use the [Tusella MCP connector](https://tusella.com/etsy-mcp-server/).

## License

MIT. Use, change and share them. Etsy is a trademark of Etsy, Inc.; this project isn't affiliated with Etsy or Anthropic.
