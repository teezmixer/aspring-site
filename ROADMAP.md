# Aspring.ca redesign: roadmap (v2, 2026-10-09)

**Goal:** redesign aspring.ca "to a completely new level": elegant, high-quality, mobile-first, with much better SEO. It stays in the **existing Wix Studio Premium project**, in **three languages (FR default, EN, UK)**. The content is what exists now, redesigned. No new features are requested.

**Pipeline (decided):**

```
Claude Design  →  Figma  →  Wix Studio (import)  →  final tweaks in Wix
 (90% of work)    (minimal)   (sandbox branch)       (multilingual text, native blocks, SEO fields)
```

Claude Code is used where code beats clicking: the SEO audit, and the copy/translation files. The GitHub repo is optional (see section 6).

---

## 1. Facts and constraints

| Topic | Fact |
|---|---|
| Wix repo / Git Integration | Syncs **Velo code only**. Page code files are empty stubs, so there's nothing to lose. Design is **not** in the repo. |
| Import tool | Wix's **Figma to Wix Studio** plugin: Studio → Tools → Import from Figma. Imports styles (fonts, colors) and frames as Page / Section / Container / Stack. Frames over 1001px wide to import as a Section or Page. Frame width should match the Studio editing size. Custom fonts must be uploaded to Studio first. |
| iframes | HTML embeds are iframes and are bad for SEO. Not used. |
| Premium plan | Can be reassigned only to another **Studio** site (confirmed by you). Not to Headless. So we stay on Studio. |
| Branches | The project has the **published site** and **one unpublished "sandbox" branch**. You couldn't create a second one. The client already started redoing the site in the existing sandbox. |
| Payments | **None.** Booking links go to **ClinicSense** (external). Intake form records stay in ClinicSense. |
| Blog | Native Wix Blog. **Keep it** (the client has started posting again). |
| Retreats | Standalone external site. Scope to confirm. |
| Holistiq (AI assistant) | Unreleased, about a year old, exists on the live site but not in the sandbox. Scope to confirm. |
| Fonts | Logo uses **Proprietor Roman**. Body text is **Montserrat**. Montserrat covers Latin Extended and Cyrillic. |
| Colors | **Dark green `#1A3320`** and **beige `#F5F5DA`** are fixed. **Sage `#3D7A56`** and any others can change for the best design. |
| Logo | Recreated in Figma, with the color switching by background. Export light and dark SVG variants. |

## 2. Scope (to confirm with the client)

| Page | Live URL (FR) | Notes |
|---|---|---|
| Home | `/` | In scope |
| Our Team | `/about-us`, `/our-mentors` | In scope. Check the difference between the two |
| Services | `/our-services` | In scope. Booking buttons go to ClinicSense |
| Contact | (form/footer, `/book-session`) | In scope. Confirm which form to keep |
| FAQ | `/faq-holistiq` | Content is Holistiq-related. Confirm |
| Blog (index + post template) | `/blog`, `/post/…` | Keep. Native Wix Blog, see section 5 |
| Pricing plans | `/pricing-plans/list` | Probably remove, since no payments. Confirm |
| Plan customization | `/plan-customization` | Likely Holistiq. Confirm |
| Holistiq | `/holistiq` | **Ask:** redesign, leave or remove |
| Retreats | `/book-retreat`, external site | **Ask:** redesign or leave |

## 3. Questions for the client (send first)
1. Which pages should be redesigned? (see the table above)
2. Is Holistiq and its AI assistant still wanted? Should it come back in the redesign or be dropped?
3. Retreats: redesign it, link to it, or leave it alone?
4. Online payments, shop or online services needed? (Assumed **no**: all booking goes through ClinicSense.)
5. Is it OK to **overwrite the sandbox** where she started redoing the site? Does she need anything from it saved first?
6. Does she edit page text herself, or do you handle all updates?
7. Does she have her own Proprietor Roman license (or Adobe Fonts) for web use? If not, the logo stays as an image and headings use a licensed font.
8. Anything she wants to keep, change or remove in the content (team bios, reviews, prices)?
9. Who owns the ClinicSense links, and do they change?

## 4. Phases

**Phase 0: Pipeline test (do before designing everything).** One test page, ideally Home's hero + a card grid, desktop and mobile:
1. Design in Claude Design. Test whether it **exports to Figma directly**. If not, fall back to HTML → Figma through the Figma tools available in Claude Code.
2. Check the Figma result (auto layout, text styles, fonts).
3. Import into the **sandbox** (Tools → Import from Figma).
4. Check the result: headings (H1/H2 can be set per text element in Studio), fidelity, **mobile breakpoint on a real phone**, fonts, how text translates in Multilingual.
5. Check what **merging the sandbox into main** does (whole-site replacement? multilingual? SEO settings? URLs?). **Do not merge anything until this is understood.** Ask Wix support if it isn't clear.
6. Output: go/no-go and a list of Figma-structure rules ("always auto layout, name layers like X") for Claude Design.

**Phase 1: Foundation (Claude Design).**
- Brand kit: logo variants, `#1A3320`, `#F5F5DA`, sage and supporting tones, tone of voice (from the email design work).
- Type: keep Montserrat for body. Choose a display font with **Latin Extended + Cyrillic** that sits well beside the Proprietor logo. Shortlist: Cormorant Garamond, Playfair Display, Lora. Test with real FR/UK text.
- Grid, spacing, components (hero, cards, therapist profile, review strip, FAQ accordion, CTA band, header/footer, language switcher).
- Mobile first: every component is designed at 390px and at desktop (over 1001px).

**Phase 2: SEO spec during design (not after).** For each page, a short spec that is designed *into* the page:
- Primary keyword and search intent.
- H1 (exactly one), H2/H3 outline, meta title (≤60 chars) and meta description (≤155 chars), in all three languages.
- Image alt text, internal links, schema type (`HealthAndBeautyBusiness`/`LocalBusiness`, `Person` for therapists, `FAQPage`, `Service`, `BlogPosting`).
- In Figma, **name layers by heading level** (e.g. `H1/Hero title`) so the hierarchy is clear after import.
- Baseline and old text come from `snapshot/` in this repo. The 12-of-13 missing meta descriptions and the heading problems are listed in the snapshot files.

**Phase 3: Page designs (Claude Design).** Order: Home → Services → Our Team → Contact → FAQ → other confirmed pages. Each as desktop + mobile frames with real copy in the three languages.

**Phase 4: Figma → Wix sandbox.** Import styles first, then each page. Replace the sandbox content with the new design (after the client OKs it). Fix heading tags, set SEO fields, enter FR/EN/UK text, and add native blocks.

**Phase 5: Blog** (see below), then **SEO check** (see section 6).

**Phase 6: QA and launch.**
- Compare every page with `snapshot/` (nothing lost), on a real phone and desktop.
- Check forms, the ClinicSense links, the language switcher and 301 redirects for any URL that changed.
- Merge or publish the sandbox (after Phase 0's findings). Verify the live site, Search Console and the sitemap.

## 5. Blog
The Wix Blog is a native app, and its feed and post pages use Wix's own templates, so the Figma import isn't the right tool for them. Plan:
- Design the blog index and post page in Claude Design as the **visual reference**.
- In Wix, apply them with the Blog's own design settings (fonts, colors, layout preset) and the shared header and footer that came in through Figma, with CSS as a polish step if needed.
- Existing posts stay. Add `BlogPosting` schema, alt text and meta descriptions.

## 6. SEO and the repo
- **Design stage:** SEO structure goes into each page's spec (Phase 2).
- **After import:** a **Claude Code SEO check** that fetches the rendered HTML (published or preview URL) and verifies H1 count, titles, descriptions, schema, `hreflang`, alt text, canonical tags and sitemap. An unpublished sandbox isn't crawlable, so this check needs a published or preview URL, or screenshots/exports of the editor.
- **The repo is the shared home for the design work.** Claude Design (connected to the design system) and Claude Code both read and write it. It holds: `brand/tokens.md` (colors, type, voice), `snapshot/` (the "before": text, SEO and screenshots for FR, EN, UK), the per-page SEO spec and three-language copy files, the design-system source, and optional Velo `wixSeo` code if setting meta tags from code turns out faster than typing them in Wix.
- **Blog page in the design:** include a placeholder blog page with the real header and footer. In Wix, the native Blog block fills the main area.

## 6a. Pipeline tools to evaluate in Phase 0
- **Claude Design → Figma:** direct export if Claude Design offers it. Otherwise **Anima** (Claude/HTML → Figma) or the Figma tools available in Claude Code. Pick whichever keeps auto layout, text styles and layer names intact.
- Test criteria for each: auto layout preserved, fonts mapped, layer names kept, and a clean mobile frame.

## 6b. Fonts (decision for the design system)
- **Body:** Montserrat (weights 300-600), already used in all 36 emails and fully Latin Extended and Cyrillic.
- **Display:** pick from Cormorant Garamond (first choice: light, luxurious, pairs well with Montserrat 300), Playfair Display, Lora. **Verify Cyrillic and French accents in the specimen**, then test beside the logo with real FR and UK headlines.
- Budget: two families, 3-4 weights.
- Upload to Studio before the Figma import so styles map correctly.

## 7. Tomorrow
1. Send the client questions (section 3) and gather her materials.
2. Finalize the scope table and the roadmap.
3. Start Phase 0: choose the test page and the pipeline path (Claude Design → Figma).
