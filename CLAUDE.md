# Project instructions

## Character sync file (`uploads/For real!_.txt`)
Whenever the user uploads (or re-uploads) this text file:
1. Read it in full and cross-reference every character/entry against the slides in `Characters.dc.html` (and any other relevant pages, e.g. Supernatural lore). Character and divider slides are written directly in that file; the arcana deck lives in `Arcana.dc.html` (the `ARCANA` array in its logic script; bearer links use character slide labels).
2. Update anything that changed — text must match the file exactly (bios, quotes, profile/vitals fields, arcana, persona, etc.). Leave unchanged content and layout alone.
3. For any NEW character not yet in the deck: add a character slide in the right section (following the existing slide pattern), a nav target in `renderVals()` (`targets` is grouped by section in deck order; keys are `go` + full name in PascalCase, e.g. `goUtakoYamanashi`, dividers use `to…`; add a `<!-- Name -->` comment above the slide and keep `data-screen-label` numbers sequential), and an `ARCANA` bearer entry in `Arcana.dc.html` if it has an arcana; then tell the user to upload their character image(s). Use a placeholder until the image arrives.
4. Keep slide order: sections go Title → Main Party → Personas → Velvet Room → Confidants → Normal Characters → Shadows → Adversaries (divider numbers 01–07 follow this). Within each section, characters are sorted by arcana in `ARCANA` array order (EX arcana sit right after their base, e.g. Councillor after Magician); Personas follow their user's party order; characters without an arcana go after those with one. Insert new characters at their sorted position and mirror that order in the divider's name list.
5. Open note: divider name lists show "—" for Chuuzenji (Tower, XVI) and the Councillors (I) — ask the user whether to fill in numerals.
6. Briefly report what was updated, what was added, and which images are still needed.
