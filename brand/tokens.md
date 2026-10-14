# Aspring brand tokens

Extracted 2026-10-09 from the confirmed email templates (`Aspring Email Marketing/html mail templates/`, 36 files, FR + EN) plus the logo and client brief. Counts are usage frequency across the templates.

## Voice
Warm, elegant, personal. Never pushy or salesy. Luxury spa tone, think high-end retreat, not a clinic. Short paragraphs, breathing room. Signature in emails: "Warmly, Victoria, Galina & Tatiana. Your Aspring Team".

## Color

| Role | Hex | In emails | Notes |
|---|---|---|---|
| Dark green (primary) | `#1A3320` | 240 | Fixed by client |
| Beige (primary light) | `#F5F5DA` | 226 | Fixed by client |
| Sage | `#3D7A56` | 90 | Changeable |
| Mid green | `#4A7A5A` | 180 | Changeable |
| Soft green | `#6A9A7A` | 180 | Changeable |
| Deepest green | `#0D2913` | 108 | Changeable |
| Deep beige | `#EDEBD3` | 82 | Surface tone |
| Muted khaki | `#C8C8A0` | 54 | Borders and dividers |
| White | `#FFFFFF` | 61 | Use sparingly |

Other greens in use (`#1F4D2A`, `#1A3D20`, `#3D5C47`, `#2E5138`, `#2E5A38`) are near-duplicates of the above. Consolidate them when building the site palette.

The logo switches between beige and dark green depending on the background.

## Type
- **Rule:** body copy is sans-serif for readability. Serif only for headings and accents.
- **Body:** Montserrat, weights 300, 400, 500, 600, plus italic 300/400. Fully Latin Extended and Cyrillic.
- **Display:** none on the web yet. The emails use Georgia as a safe stand-in for headings, and the logo is set in Proprietor Roman.
- **Display:** Cormorant Garamond (also used in the client's own mockup). Alternatives: Playfair Display, Lora.
- Client mockup used Work Sans for body. Montserrat is already in the 36 emails and live site, so it is the default unless a side-by-side says otherwise.
- Budget: two families, 3-4 weights, for mobile load speed.

## Languages
**English (default) and French only. Ukrainian is dropped** (confirmed 2026-10-14). The current live site is French-default with `/en` and `/uk`, so URLs need redirects. Cyrillic is no longer required, only French accents (Latin Extended).

## Client draft palette (reference only, to be standardized)
From her mockup/spec: cream `#FAF8F3`, warm panel `#F2EDE2`, light sage `#E6EDE3`, accent sage `#546B52` (hover `#41543F`), dark green `#3A4B3C`, text `#35322A` / `#57514A` / `#6E675E`, borders `#E6E2DA`, decorative blobs `#D7E4D4` and `#EFDDCB`. These are close to, but not the same as, the email palette above. They get merged into one scale around `#1A3320` and `#F5F5DA`.
