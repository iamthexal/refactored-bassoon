# Project instructions

## Character sync file (`uploads/For real!_.txt`)
Whenever the user uploads (or re-uploads) this text file:
1. Read it in full and cross-reference every character/entry against the slides in `Characters.dc.html` (and any other relevant pages, e.g. Supernatural lore). Character and divider slides are written directly in that file; the arcana deck lives in `Arcana.dc.html` (the `ARCANA` array in its logic script; bearer links use character slide labels).
2. Update anything that changed — text must match the file exactly (bios, quotes, profile/vitals fields, arcana, persona, etc.). Leave unchanged content and layout alone.
3. For any NEW character not yet in the deck: add a character slide in the right section (following the existing slide pattern), a nav target in `renderVals()`, and an `ARCANA` bearer entry in `Arcana.dc.html` if it has an arcana; then tell the user to upload their character image(s). Use a placeholder until the image arrives.
4. Briefly report what was updated, what was added, and which images are still needed.
