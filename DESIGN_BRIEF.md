# Design brief: aspring.ca

**Read this first.** It tells you what to build, which files are authoritative, and which rules the Wix import imposes. Everything else in the repo is referenced from here.

---

## 1. The job

Redesign the website of **Aspring Health Center**, a massage therapy, naturopathy and Ayurveda practice in Plateau-Mont-Royal, Montréal, run by **Victoria**, who is the founder and the only practitioner. The new site replaces an old, inconsistent one and has to:

- feel **calm, elegant, uncluttered and not old-fashioned**: a high-end retreat, not a clinic
- **convert**: a visitor lands, feels it, and wants to book a session
- be **excellent on mobile first**, then tablet and desktop
- be **bilingual: English (default) and French**
- be built so that Victoria can **edit the text herself later** in Wix Studio

The design ends up in **Wix Studio** through Figma ("Import from Figma"). Section 6 lists the rules that makes that import work. Follow them from the first frame.

## 2. Sources of truth, in order

| File | Use it for | Authority |
|---|---|---|
| `DESIGN_BRIEF.md` (this file) | Structure, rules, scope | Highest |
| `CONTENT.md` | **Every word on every page** (EN + FR), each block tagged by source | **Only source of text** |
| `brand/tokens.md` | Colors, type, voice, extracted from the approved emails | Brand |
| `FACTS.md` | Numbers, hours, contacts, prices, and which are still unconfirmed | Facts |
| `content/source/clinicsense-services.json` | Real service names, durations, prices | Prices only. Descriptions here are unsoftened, so use the website versions in `CONTENT.md` |
| `client-brief/mockup-full-site.html`, `spec-harmony-v1.txt` | The client's own draft: **layout and mood reference only** | **Not authoritative.** Her draft prices, testimonials, credentials and dates are partly invented. Her colors and fonts are suggestions |
| `snapshot/screenshots/` | How the old site looked (desktop and mobile) | "Before" reference |
| `new logo aspring beige.svg` / `.png` | Logo, beige version | Brand |

**Text rule:** use only the text in `CONTENT.md`. Do not write, reword or invent copy in the design. If something is missing, leave a clearly marked `[TEXT NEEDED: …]`. Blocks tagged `PLACEHOLDER` are dummy content to make the layout reviewable and must be visibly marked as placeholders in the design. Blocks tagged `FACT` contain numbers that are still unconfirmed, so mark them too.

## 3. Brand

### Mandatory colors (already used in all email templates)
| Role | Hex |
|---|---|
| **Dark green** | `#1A3320` |
| **Ivory** | `#F5F5DA` |

These two are fixed, and the logo switches between them depending on the background (ivory logo on dark green, dark green logo on ivory).

### Open for us to design
Everything else: the rest of the palette is **to be designed together**. Starting points from what the brand already uses (emails) and from the client's draft. Treat them as candidates, not requirements:

| Candidate | Hex | Seen in |
|---|---|---|
| Sage | `#3D7A56` | emails, buttons |
| Mid green | `#4A7A5A` | emails |
| Soft green | `#6A9A7A` | emails |
| Deepest green | `#0D2913` | emails |
| Deep ivory | `#EDEBD3` | emails, panels |
| Muted khaki | `#C8C8A0` | emails, borders |
| Client's draft accent | `#546B52`, with `#3A4B3C`, `#E6EDE3`, `#F2EDE2` | client mockup |

The email and client palettes overlap with several near-duplicate greens. **Consolidate into one named scale** (a few greens, a few ivory/neutral tones, text colors). Check that all text and button combinations meet **WCAG AA contrast** (4.5:1 for body text).

### Type
- **Headings: Cormorant Garamond** (regular and italic for accents; weight regular, not bold)
- **Body: Montserrat**, which is already in all emails (weights 300, 400, 500, 600)
- **Rule: body copy is always sans-serif** for readability, especially on phones. Serif is for headings and accents only.
- Two families, three to four weights in total, for load speed.
- Languages are English and French only, so **Latin Extended** (accents) is required and Cyrillic is not.
- Montserrat is the default body font unless a side-by-side with the client's draft font (Work Sans) shows a clearly better result.

### Voice
Warm, elegant, personal, in the first person for Victoria. Short paragraphs, breathing room. Never pushy or salesy. No bullet-point heaviness. (Full notes in `brand/tokens.md`.)

### What the client said she wants (her words, summarized)
Calm, elegant, **not cluttered**, **not old-fashioned**, professional and tidy. Designed well, but it must actually **work and convert**. **SEO built in.** **Mobile, tablet and desktop** all checked. Consistent facts everywhere.

## 4. Site structure

### Header (shared)
- Left: wordmark **Aspring Health** with a small line "Holistic Care · Montréal"
- Centre: **Massage Therapy · Naturopathy & Ayurveda · Retreats · Events · Digital Library**
- Right: **EN / FR** switcher, then the primary button **Book a Session** (links to ClinicSense, opens in a new tab)
- Sticky on scroll. A cart icon exists **only on the hidden Shop page**.
- Mobile: a clean menu pattern, with the Book button always reachable.

### Footer (shared)
Four columns: name and one-line description; contact block (address, phone, email, hours); navigation; newsletter signup. Bottom row: copyright "© 2026 Aspring Health Center", social links (Instagram, Facebook), privacy policy. **Journal (blog)** is linked from the footer navigation (a design decision to review, since the client's spec has no blog link).

### Pages (build in this order)
1. **Home**: hero (H1 "Come home to your body."), stats band, philosophy with credentials, three featured service cards, testimonials, closing call to action. It also has to carry Victoria's story and credibility, because the old About page is gone.
2. **Massage Therapy**: intro, **7 real services** with durations and prices (a repeating list), insurance/trust card, booking section.
3. **Naturopathy & Ayurveda**: intro, **5 real services**, consultation process, credentials, related products (placeholder).
4. **Retreats**: split hero, upcoming retreats (two cards), past retreats gallery (six), inquiry form.
5. **Events**: calendar-style list with category chips, registration, private-group inquiry band.
6. **Digital Library**: instant-download product grid, how-it-works band.
7. **Shop**: built but **hidden from the menu**.
8. **Blog**: a placeholder page with the real header and footer. A native Wix Blog block fills the main area later.

Pricing and services are **repeating rows/cards, not a Wix table**, so they can be connected to Wix's database later.

## 5. Native Wix blocks: design clear placeholders

Some parts of the site are **Wix apps** and can't be imported from Figma. Design each as a **clearly labeled placeholder** tagged **"Native Wix block"**, so Victoria can review the full experience before anything is built in Wix:

- Product page, cart, checkout, order-complete (Wix Stores, for the Library and Shop)
- Event detail and registration (Wix Events)
- Blog index and blog post (Wix Blog)
- Forms: **newsletter** (footer), **retreat inquiry** (name, email, phone, which retreat, message), **private-group inquiry**, and their thank-you states (Wix Forms)
- **Booking**: an external ClinicSense link, shown as a button, not a widget

Match the site's look in these placeholders as far as reasonable, but expect Wix's own styling controls to limit what's possible.

## 6. Rules so the Figma → Wix Studio import works

The importer converts Figma frames into native, responsive Studio elements. Design for that:

1. **Frame widths:** desktop **1440 px** (the importer requires frames wider than 1001 px for pages/sections), **tablet 768 px**, **mobile 390 px**. Studio's exact breakpoints are checked in the pipeline test.
2. **Auto layout everywhere.** Build with nested auto-layout frames, as you'd write flexbox. Avoid free-floating, absolutely positioned layers except for purely decorative shapes.
3. **Real text.** All text is live text, never text baked into an image.
4. **Name layers by role**, and by heading level: `H1/Hero title`, `H2/Section title`, `Body/Lead`, `Button/Primary`, `Image/ah-svc-massage`. One **H1 per page**, then a logical H2 → H3 hierarchy.
5. **Reusable components** for header, footer, buttons, cards, rows, chips and forms, with variants for desktop/tablet/mobile.
6. **Tokens, not hard-coded values:** colors, type styles, spacing and radii defined once as Figma variables/styles, so the import brings in a clean style set.
7. **Keep effects simple.** Prefer solid fills and thin borders. Test anything fancy (blurs, backdrop filters, gradients, shadows, animations) in the pipeline test before relying on it. Wix may drop it.
8. **Images:** each image is a named slot with a **proposed alt text**. Photos arrive later, from a folder the client already has, so design with placeholders that match their intended crop. **Don't use stock photos.**
9. **Plan for French.** French text runs about **20–30% longer** than English. Check headlines, buttons and the header at that length.
10. **Forms and buttons:** every button has a hover and a disabled state, and every form has an error and a success state.

## 7. SEO rules that affect the design

- **One H1 per page**, with the text given in `CONTENT.md`. Don't make the H1 an image or a logo.
- Headings follow the document outline (H1 → H2 → H3), never chosen for their size. Style and level are separate.
- Important text stays **real, visible text** in native elements. No text in images, no key content hidden in tabs or accordions that is not also in the page.
- Service pages show **durations and prices** as text.
- Meta titles and descriptions per page are drafted in `CONTENT.md` (section 10). The design doesn't need to show them.

## 8. Usability and accessibility

- **Mobile first.** Body text 16 px minimum on mobile. Tap targets 44 px minimum. The Book a Session button is always one tap away.
- Contrast to **WCAG AA**. Visible focus states.
- Calm motion only (subtle fades). No autoplay, no carousels that hide content.
- Keep the page light: restrained imagery, two font families.

## 9. Open for design

Yours to explore, with the client in the loop:
- the rest of the palette (section 3), the grid and spacing scale, the image treatment (crop, color grade, radius)
- decorative elements (the client's draft used soft blurred circles and pill-shaped buttons; keep, change or drop)
- the exact component styles, section rhythm and mobile navigation pattern

## 10. Deliverables and order of work

1. **Design system** (Figma-ready): variables for colors, type, spacing, radii; the component set with desktop/tablet/mobile variants.
2. **Home page**: desktop, tablet, mobile, in EN and with a French check on the hero, header and buttons.
3. **STOP: pipeline test.** Before designing the other pages, import this one page into the Wix Studio sandbox and check it (section 11). Findings may change the rules in section 6.
4. **The remaining pages**, in the order above, then the **native-block placeholders**.
5. A **clickable prototype** for the client to review, with native Wix blocks clearly labeled.
6. The Figma file organised for import: one page per site page, components on a separate page, a layer-naming check.

## 11. Pipeline test checklist (after the Home page)

- [ ] Auto layout survives the import
- [ ] Heading tags: is the H1 an H1? (fixable in Studio)
- [ ] Fonts: Cormorant Garamond and Montserrat load, and weights map correctly
- [ ] Desktop, tablet and **mobile on a real phone** all look right
- [ ] French text fits in the header, buttons and hero
- [ ] Which effects Wix drops (blur, shadows, gradients)
- [ ] The Book button opens ClinicSense in a new tab
- [ ] What merging the sandbox into the live site does (languages, SEO settings, URLs)

---

## Paste this to start the first Claude Design session

> You're designing the website for Aspring Health Center, a calm, elegant massage-therapy, naturopathy and Ayurveda practice in Montréal. Read `DESIGN_BRIEF.md` first and follow it exactly. Use only the text in `CONTENT.md`. Mandatory colors are dark green `#1A3320` and ivory `#F5F5DA`; the rest of the palette is for us to design together. Headings are Cormorant Garamond, body is Montserrat. Build in auto layout with named layers so the design imports cleanly into Wix Studio via Figma. Start with the design system, then the Home page at desktop 1440, tablet 768 and mobile 390, and stop for review before the other pages.
