# Project instructions

## Offline data copy
After ANY change to `data/*.json`, regenerate `data/offline-data.js` (`window.PRP_DATA = {characters, groups, arcana, layout}` — the four files' parsed contents). The deck falls back to it when opened from an unzipped folder, where the JSON can't be fetched.

## Character sync file (`uploads/For real!_.txt`)
Whenever the user uploads (or re-uploads) this text file:
1. Read it in full and cross-reference every character/entry against the deck data in `data/` (and any other relevant pages, e.g. Supernatural lore). Character/divider slides are generated from `data/characters.json` (content), `data/groups.json` (sections + order), `data/arcana.json` (arcana deck + bearers) and `data/layout.json` (all positioning numbers) — edit the JSON, not the slide markup.
2. Update anything that changed — text must match the file exactly (bios, quotes, profile/vitals fields, arcana, persona, etc.). Leave unchanged content and layout alone.
3. For any NEW character not yet in the deck: add an entry to `data/characters.json`, its id to the right group's `members` in `data/groups.json` (and `bearers` in `data/arcana.json` if it has an arcana), plus a `data/layout.json` entry; then tell the user to upload their character image(s). Use a placeholder until the image arrives.
4. Briefly report what was updated, what was added, and which images are still needed.
