# Aspring.ca redesign: technical roadmap (v3, 2026-10-14)

**Goal:** redesign aspring.ca "to a completely new level" (elegant, high-quality, mobile-first, much better SEO), **inside the existing Wix Studio Premium project**, with the client's new functions added: digital products, retreat sign-up and events registration.

**Pipeline:**

```
Claude Design (+ Claude Code)  →  Figma  →  Wix Studio sandbox (Import from Figma)  →  native setup in Wix
      ~60% of the work             ~5%                  import + fixes                    ~35% of the work
```

(The percentages are rough and get refined after Phase 0.)

---

## 1. Ground truth

### Client input (in `client-brief/`)
- `spec-harmony-v1.html/.txt`: the client's own spec (Russian). **Draft only, free to change.** Written for Wix Harmony and its AI agent, so the agent prompts, the Harmony setup steps and the domain-connection steps are **ignored**. We keep: pages, section structure, functions table, CMS ideas, photo list, pre-launch checklist.
- `mockup-full-site.html`: her 7-page prototype (EN/FR toggle, fake checkout modal). `mockup-digital-library-checkout.html`: library checkout flow. Both are **reference only**. They use her own palette and Work Sans.

### Decisions
| Topic | Decision |
|---|---|
| Platform | **Wix Studio** (Premium plan can only move to another Studio site). Not Harmony, not Headless. |
| Domain | Stays as is. No transfer needed. |
| Languages | **English (default) + French only. Ukrainian is dropped.** |
| Booking | Stays on **ClinicSense**: every "Book a Session" button links externally to `victorianosenko.clinicsense.com/book/` in a new tab. Wix Bookings is not needed. |
| Email marketing | **Brevo** for all automations and communications. What she wants from it is still to be clarified, but it doesn't block design. |
| Blog | Keep (native Wix Blog), restyled. Placeholder page with the real header and footer in the design. |
| Name | **Aspring Health Center** everywhere (matches the Google Business Profile); the header wordmark says **Aspring Health**. |
| Design brief | **`DESIGN_BRIEF.md`** is the single entry point for Claude Design: sources, rules, page order, import rules, pipeline-test checklist. |
| Text | **`CONTENT.md` is the ground-truth text for the design** (EN + FR, tagged by source). Real service data is in `content/source/`. |
| Fonts | Body is **sans-serif**, serif only for headings and accents. Direction: **Cormorant Garamond** (display, already in her mockup) + **Montserrat** (body, already in your 36 emails and the live site). Her mockup uses Work Sans: Montserrat is the closer match to the existing brand, so the final choice needs a quick check. Cyrillic is no longer required, only French accents. |
| Colors | **Dark green `#1A3320`** and **beige `#F5F5DA`** fixed (from the emails). Her draft shades (`#FAF8F3`, `#F2EDE2`, `#E6EDE3`, `#546B52`, `#3A4B3C`, `#35322A`, `#57514A`, `#6E675E`, `#E6E2DA`) are standardized into one palette in the design-system step. Not now. |
| Branches | Published site + one unpublished **sandbox**. **Overwriting it is approved by the client.** |
| Plan | **Wix Studio Standard**, which allows all needed functions (Stores, payments, Events, Forms). Names differ from the generic tier names. Verify checkout can accept CAD payments before relying on it. |
| Pages | **Only the new spec.** The old site is deprecated. Old pages that disappear get 301 redirects. **Facts from the old site must stay consistent** (see `FACTS.md`). |
| Voice | **Victoria only**, the founder and the only working therapist. Remove Halina from the site.  The current emails already sign as Victoria only. |
| Editing | **The client edits the site herself**, so it stays on Studio with native elements: no iframes for text, minimal custom code, nothing that breaks when she edits a text box. |
| Photos | All exist. The folder goes to Claude Design to fill the layouts, after the design is done. |
| Logo | Image only (no Proprietor Roman web license). Real text never uses that font. |
| Products / events | Draft placeholders from her mockups are the content for now. Real products to be clarified later. Events and retreats are only the ones in the drafts. |

### Pages from her spec (replaces the earlier scope table)
| # | Page | Notes |
|---|---|---|
| 1 | Home | Hero, stats band, philosophy, featured services, testimonials, closing CTA |
| 2 | Massage Therapy | Five massage types, pricing table, insurance card, booking |
| 3 | Naturopathy & Ayurveda | Services, consultation process, licenses, related products |
| 4 | Retreats | Upcoming + past retreats, inquiry form |
| 5 | Events | Calendar-style list with category filter, registration |
| 6 | Digital Library | Product grid, purchase and download (new) |
| 7 | Shop | Created but **hidden from the menu**, cart icon only on this page (new, later) |
| + | Blog (index + post) | Keep. Native |
| + | Header / footer | Shared. Includes the EN/FR switcher and a Brevo newsletter form |

**Dropped (decided):** About/Team, FAQ, Contact, Book Session, Holistiq/AI assistant, Pricing Plans, Plan Customization and everything under `/uk`. Each old URL gets a **301 redirect** to the closest new page, so the existing rankings on aspring.ca carry over. The new site stays on the same domain, because it is already indexed well. The redirect map is a Phase 3 deliverable.

### What Victoria asked for (her words, summarized)
- **Calm, elegant, uncluttered. Not old-fashioned.** Professional and tidy.
- **It has to convert.** A visitor lands, feels it, and wants to book a session.
- **SEO built in**, with all texts rewritten to be SEO-strong (titles, headings, descriptions, alt text).
- **Same domain.** It is already indexed well, hence the 301 redirect plan.
- **No contradictions.** Same years of experience, same opening hours and the same facts everywhere (`FACTS.md`).
- **Checked on mobile, tablet and desktop.** Mobile matters most because many visitors use it.
- **Bilingual:** English and French.


## 2. Functions → where they are built (her section 6)

| Function | Wix feature | Needs | Built in |
|---|---|---|---|
| Book a Session | External link to ClinicSense | Nothing | Design / button link |
| Digital Library (e-books, guides) | **Wix Stores → digital products** | Business plan, payment provider | **Wix native** (design reference from Claude Design) |
| Shop (hidden, later) | Wix Stores | Same | Wix native |
| Payments | Wix Payments or Stripe | Business plan, **CAD** as main currency | Wix native |
| Retreat interest / inquiry form | Wix Forms (email notification + autoresponder) | Nothing | Wix native |
| Event registration | **Wix Events** (RSVP, tickets, reminders) | Payments if tickets are paid | Wix native |
| Newsletter, retreat interest, behavior data | **Brevo** (replaces her "Wix Email Marketing") | Brevo account | See section 3a |
| EN / FR | **Wix Multilingual** (EN default) | Nothing | Wix native: translations entered manually |
| Retreats / events / books / testimonials / services as repeatable cards | **Wix CMS** (optional) | Nothing | See section 3 |
| Blog | Wix Blog | Nothing | Wix native, restyled |

**Plan:** Studio Standard allows all the functions above. Remaining check: a test purchase and download in the sandbox before launch.

**Native widgets can't come in through Figma.** Stores product pages, cart, checkout, Events, Forms internals and the Blog are Wix apps. Design them in Claude Design as a visual reference, then match them in Wix with each app's design settings plus the shared header, footer and styles that did come through Figma. The prototype's fake checkout modal is only a mock. **Claude Design builds a clearly labeled placeholder for every native block** (product page, cart, checkout, event detail and registration, blog index and post, forms, newsletter form, thank-you states), tagged "Native Wix block", so Victoria can review the whole experience before anything moves to Wix.

## 3. CMS in plain terms
Wix CMS is a built-in database. You make a **collection** (a table: e.g. "Retreats" with name, dates, price, photos) and bind a **repeater** or **dynamic page** to it in the editor. Adding a retreat then means adding a row, with no layout work, and each item can get its own URL and SEO fields.

Recommended (keep it small, because every collection is manual binding work in Wix):
- **Use CMS for:** Retreats (upcoming vs past), Testimonials, Services/pricing table (EN and FR text per row).
- **Don't need CMS for:** Events (Wix Events has its own data), Library/Shop (Wix Stores has its catalog), Blog (native).
- The rest of the content stays as static page content.

Collection data can be prepared in this repo (CSV/JSON in EN and FR) and imported, so no one retypes it.

**You don't need a separate page per collection.** A collection is just data. You place a repeater (cards, rows, gallery) on any existing page, such as Testimonials on Home, the pricing rows on Massage, Upcoming and Past on Retreats, and connect it to the collection. A separate *dynamic item page* (one URL per row, e.g. one page per retreat) is only needed if you want each item to have its own URL, and it can be added later. Design implication: build the pricing table as repeating **rows**, not a Wix Table element, so it can be connected to the collection.

## 3a. Brevo ↔ Wix: one contact database
Goal: all contacts end up in Brevo, so retreat announcements, flows and segments live in one place.

**Decision: Wix native forms only, no second set of Brevo forms.** Every form on the site is a Wix Form (or a Wix app's own form). Submissions are copied to Brevo by a small script or connector, so there's one form to design, test and maintain per use case. The sync options, simplest first:

1. **Velo backend script (code in this repo).** When a Wix form is submitted, a backend handler calls Brevo's API to create or update the contact (matched by email) and set attributes, such as `RETREAT_INTERESTED = yes` or adding to a list. The Brevo API key is stored in Wix's Secrets Manager. The same pattern later covers event registrations and digital-product purchases (`LAST_EVENT_ATTENDED`, `DIGITAL_PRODUCTS_BOUGHT`), which is your behavior-data idea. **To verify:** the exact backend event Wix offers for form submissions, and that Brevo's "create or update contact" call updates existing contacts without duplicating.
2. **Connector tools** (Zapier, Make, Outfunnel). Third-party listings show Wix Forms, Events, eCommerce and CMS forms as triggers that add or update Brevo contacts ([Zapier](https://zapier.com/apps/brevo/integrations/wix/255613794/manage-cms-forms-in-wix-to-add-or-update-contacts-in-brevo), [Outfunnel](https://outfunnel.com/brevo-wix-forms-integration/)). They add a monthly cost, so use them only if option 1 turns out to be too much work.

I did not find documentation of an official Brevo plugin for Wix, so check Brevo's help center and the Wix App Market before relying on that route.

**Forms the design needs, and where each lands:**

| Form | Where | Sync to Brevo |
|---|---|---|
| Newsletter | Footer | New contact → newsletter list |
| Retreat interest / inquiry (name, email, phone, which retreat, message) | Retreats page | Contact + `RETREAT_INTERESTED = yes` |
| Event registration | Events (Wix Events) | Contact + event attended (later) |
| Digital product purchase | Library (Wix Stores) | Contact + product bought (later) |
| Private group session inquiry | Events page closing band | Contact + tag |

The newsletter and retreat forms are priority one. Event and purchase behavior can come later.

## 4. Work split

| Where | What |
|---|---|
| **Claude Design + Claude Code (~60%)** | Design system (brand tokens, fonts, components). All pages desktop + mobile in EN and FR, with real copy. SEO spec per page (H1, outline, meta title/description, schema, alt text). Redirect map (old URL → new URL, including `/uk`). Placeholder blog page, library/shop/checkout visual references. CMS data files. Final SEO audit scripts. |
| **Figma (~5%)** | Receives the export. Check auto layout, text styles, layer names (`H1/…`). Light cleanup only. |
| **Wix Studio (~35%)** | Upload fonts, import styles, import pages from Figma into the sandbox. Set heading tags, fix mobile breakpoint. Multilingual: enter FR text. Stores (digital products, payments, CAD, taxes), Events, Forms + notifications, CMS bindings, Blog styling, Brevo form, redirects (CSV import), SEO fields. Final publish. |

## 5. Phases

**Phase 0: Pipeline test, before designing everything.** One page (Home hero + a card grid), desktop and mobile. Claude Design → Figma (direct export, Anima, or the Figma tools in Claude Code) → Studio sandbox. Check: headings, auto-layout fidelity, mobile on a real phone, fonts, how EN/FR text behaves in Multilingual. Also check what **merging the sandbox into main** does (multilingual, SEO settings, URLs). Don't merge before this is understood.

**Phase 1: Scope lock.** Page list is decided (section 1). Fill `FACTS.md` with Victoria (section 7).

**Phase 2: Design system.** Brand tokens (`brand/tokens.md`), fonts, palette standardization, components, mobile-first. Frames over 1001px wide for import.

**Phase 3: SEO spec (during design).** Per page: primary keyword, H1, heading outline, meta title (≤60) and description (≤155) in EN and FR, alt text, schema (`HealthAndBeautyBusiness`, `Service`, `Person`, `Event`, `Product`, `BlogPosting`, `FAQPage`), internal links. Redirect map. Old-site baseline is in `snapshot/`.

**Phase 4: Page designs.** Order: Home → Massage → Naturopathy → Retreats → Events → Digital Library → header/footer → blog placeholder → Shop. EN and FR copy for each, desktop, **tablet** and mobile. Native-block placeholders (see section 2) are included. **Review with Victoria as a clickable HTML prototype before moving anything to Wix.**

**Phase 5: Figma → Wix sandbox.** Import styles, then pages. Per-page checklist: heading tags, mobile, SEO fields, FR text.

**Phase 6: Wix apps.** Business plan check, Stores + payments, Events, Forms, CMS, Brevo form, Blog styling.

**Phase 7: SEO check with Claude Code.** Fetch the rendered HTML from a published or preview URL: H1 count, titles, descriptions, schema, `hreflang`, canonicals, alt text, sitemap, redirects.

**Phase 8: QA and launch.** Compare against `snapshot/` (nothing lost), real-phone tests, test purchase and download, form notifications, ClinicSense links in new tabs, address consistency (415 Boul. Saint-Joseph Est), Search Console. Merge or publish.

## 6. SEO notes
- **English as the default** changes the URL structure: today `/` is French and `/en` is English. We decide what `/` serves, where French lives, and add 301 redirects, updated `hreflang` and `x-default`. Check search demand in French vs English for Montréal before locking.
- Missing meta descriptions (12 of 13), missing/duplicate H1s and thin schema on the current site are in `snapshot/`.
- Native Stores/Events/Blog pages get their SEO from each app's own settings, so those fields are Wix-native work.

## 7. Open items

**Answered (2026-10-14):** pages (new spec only), voice (Victoria only), payments (yes, products still to clarify), events and retreats (only the drafts), photos (all exist), sandbox (overwrite OK), languages (EN default + FR), client edits herself (so Studio), logo (image only), Brevo approach (your call).

**Still open:**
1. **Facts for `FACTS.md`:** contact details and prices are now filled from the approved email and ClinicSense. Still needed: years of experience, hours of practice, clients vs. sessions (950), rating, credentials, the Monsalada wording, and which services appear on the site.
2. **ClinicSense text cleanup (Victoria):** the neck-therapy description names "Andrey Aspring" and several service texts make strong health claims. The website versions are already softened in `CONTENT.md`; fixing ClinicSense keeps both consistent.
3. **Products:** what the Digital Library and Shop actually sell (the drafts are placeholders).
4. **Brevo:** which forms to build first (section 3a) and test the contact-update behavior.
5. **Social URLs and email address** for the footer.

## 8. Next
1. Fill `FACTS.md` with Victoria.
2. Run Phase 0 (one page through Claude Design → Figma → sandbox, desktop, tablet and mobile).
3. Design the system, then the pages and the native-block placeholders.
