---
name: research-place
description: Research a city, town, county or region for service-area pages and save the findings to its note in places/. Use when asked to research, look up, or build local knowledge for a place, e.g. "/research-place hialeah florida".
---

# Research a place

Input: place name and state (ask if the state is missing).

1. **Find the note.** Look for `places/<state>/<place>.md` (lowercase, hyphens). If it is missing, copy `templates/place.md` there and fill `title`, `state`, `state_abbr`, `place_type`.
2. **Read what is there.** Only research sections that are empty, marked `None found` more than 6 months ago, or older than `last_checked` + 12 months.
3. **Research, in this order:**
   - Census QuickFacts / ACS: population (with year), median household income, households, county.
   - Coordinates: Census Gazetteer.
   - Industries and major employers: city or county economic development site, chamber of commerce, BLS.
   - Geography and risks: FEMA declarations, NOAA storm data, local news for floods, storms, outages.
   - Events and incidents: dated, from news or government sources, last 5 years.
   - Local business needs: construction projects, hospitals, hotels, events venues, farms, ports, camps.
4. **Write it in.** Every fact gets a numbered source with URL, publish date and access date. Nothing found → `None found (searched <today>)`.
5. **Connect it.** Fill `hub`, `county`, `industries`, `risks`. Match the place to notes in `use-cases/` and list them under `## Rental use cases` with one line each on why. Add the place to each matching use-case note's `## Places where this fits`.
6. **Update** `last_checked` to today, and add a link to the place in `places/<state>/_state.md` if missing.
7. **Report** in 5 lines or fewer: what was added, what was not found, and which use cases fit.
