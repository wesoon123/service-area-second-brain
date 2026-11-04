# Second Brain: rules for Claude

This folder is an Obsidian vault and a knowledge bank: ideas, research, SEO strategy, and local knowledge for service-area pages. You are its librarian. Answer from it, add to it, and keep it trustworthy.

## Where things go

| Folder | What lives there | File name |
|---|---|---|
| `places/<state>/` | One note per city, town, county or region | `places/florida/miami.md` (lowercase, hyphens) |
| `places/<state>/_state.md` | State-level facts: climate risks, major industries, regulations | one per state |
| `use-cases/` | One note per rental equipment type (Super 9) and the situations that need it | `use-cases/mobile-laundry.md` |
| `seo/` | Keyword research, page strategies, what ranked and what didn't | `seo/<topic>.md` |
| `ideas/` | Business and content ideas, half-formed is fine | `ideas/<short-name>.md` |
| `sources/` | Saved source summaries worth citing more than once | `sources/<publisher>-<topic>.md` |
| `inbox/` | Quick captures not filed yet | `inbox/YYYY-MM-DD-<topic>.md` |
| `templates/` | Note templates. Copy, never edit in place | |

New note: start from the matching file in `templates/`. Keep the frontmatter keys exactly as the template has them.

## Facts and sources

- Every fact in `places/` and `use-cases/` needs a source: URL, publication date (or "undated"), and access date, listed under `## Sources` and numbered `[1]`, `[2]` inline.
- Never invent a fact, figure, business name, or event. If you cannot find it, write `None found (searched YYYY-MM-DD)`. That is a valid entry and stops the next search repeating the work.
- Prefer primary sources: U.S. Census Bureau (QuickFacts, ACS), BLS, state and city government sites, NOAA/FEMA, chambers of commerce. Note when a figure is an estimate and for which year.
- When a newer figure replaces an older one, update it and keep the old one in `## History` with its date.
- Set `last_checked` in the frontmatter to today whenever you verify or add facts.

## Answering questions

1. Search the vault first (`places/`, `use-cases/`, `seo/`, then everything). Quote the note and its source.
2. Say clearly what the vault does not cover. Offer to research it; don't fill gaps from memory.
3. When you research something new, write it into the right note before answering, so it is kept.
4. Link related notes with `[[note-name]]`: a city to its county, hub city, state, and the use cases that fit it.

## Inbox

When asked to "process the inbox": move each capture into the right folder, merge it into an existing note where one fits, add links, then delete the inbox file.

## Service-area pages (trailer-site-kit)

Site repos built with trailer-site-kit read local facts from this vault:
- Before researching a place for a page, read `places/<state>/<place>.md`.
- After researching, write new facts back here with sources, then use them in the site.
- Rental use cases for a place come from matching its industries, geography and risks to `use-cases/`.
