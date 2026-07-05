# 7-5-JeremyLB-Prototype-code
code for website template
Single-page website for **Jeremy Luce Builder** — a custom home builder in Austin, Texas.

The entire site is one self-contained file: `index.html`. All CSS is inline, all images are embedded as base64, and the Russo One font is embedded. The only external resource loaded is the Space Mono body font from Google Fonts.

**No external assets, no build step, no dependencies** (except the optional Google font link, which has a bold fallback stack).

## View it locally

Just open `index.html` in any web browser (double-click it, or drag it into a browser tab).

## Publish it free with GitHub Pages

1. Create a new repository on GitHub (e.g. `jeremy-luce-builder`).
2. Upload `index.html` to the repository.
3. Go to **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Select the `main` branch and the `/ (root)` folder, then **Save**.
6. Wait ~1 minute. Your site will be live at: `https://<your-username>.github.io/<repository-name>/`

To use a custom domain (e.g. `jeremylucebuilder.com`), add it under **Settings → Pages → Custom domain**.

## Design

- **Fonts:** Russo One (wordmark/headings, embedded as base64); Space Mono (body, from Google Fonts).
- **Colors:** Red #A81E26 (header), Brown #181310 (About/Projects/Services), Cream #F5ECDD (text on dark), Green #4E6B4A (accent, sparing use).
- **Header:** Full-bleed red, wordmark left-aligned two lines (JEREMY LUCE / BUILDER), subline "Custom Homes · Austin, Texas", text nav top-right.
- **Sections:** Header → About (incl. merged Craftsmen subsection) → Projects → Services → Contact → Footer. Brown runs continuously About through Services.
- **Principle:** Timeless over trendy. Cohesive, disciplined palette. Cross-device compatible (no horizontal overflow at any width).

## What's done

- Header with embedded Russo One, full-bleed red, edge-to-edge (no white gaps).
- About section: professional B&W portrait (left, thin green border) + Big Bend hiking photo (lead, top-right) + supporting margin photos + 3 bullet facts.
- Merged Craftsmen section (3 placeholder cards, ready for real photos).
- Projects grid (14 placeholder cards — ready for 4–6 real hero projects).
- Services section, contact form (wired to nothing yet), footer.
- File size: ~1 MB. Fully self-contained except Space Mono font link.

## What's left (to-do)

1. **Projects portfolio:** Replace 14 "Photo" placeholders with 4–6 real hero projects (name + architect + photo each). Strategy: hybrid — show best builds from Jon Luce Builder (where I was on-site PM) + later add a short bridge copy explaining Jon Luce Builder (PM, ~2 decades) → Jeremy Luce Builder (mine, ~2024). *Note: bridge copy wording is deliberately tabled — craft it later.*

2. **Craftsmen section:** Replace 3 placeholder cards with curated in-action photos (name + trade for each).

3. **Contact form:** Currently does nothing. Wire to a real handler (e.g., Formspree, Web3Forms) and add real phone, email, Instagram/X links (all placeholders now).

4. **Optional:** Embed Space Mono for a 100% dependency-free file.

5. **Optional:** SEO basics — meta description, Open Graph tags, LocalBusiness structured data, favicon.

## Editing

Everything lives in `index.html`:

- All CSS is in the `<style>` block (inline).
- All images are base64-encoded in `src=` attributes.
- All fonts are either embedded (@font-face Russo One) or linked (Space Mono from Google).
- Keep the file self-contained: if you add photos, resize and compress them, then convert to base64 before embedding.

## License

© Jeremy Luce Builder. All rights reserved.
