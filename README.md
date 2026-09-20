# Concrete Pavers Dallas TX — Landing Page

Single-page, static site targeting the keyword **concrete walkways dallas tx**.
No frameworks, no build step, no dependencies. Upload the files and it runs.

---

## Files

| File | Purpose |
|---|---|
| `index.html` | The full page — styles, schema and scripts are inline (single file, fast load) |
| `robots.txt` | Crawl rules + sitemap reference |
| `sitemap.xml` | XML sitemap with image entries |
| `README.md` | This file |

> Note: the correct filename is **`robots.txt`** (with the *s*), not `robot.txt`. Search engines only read `robots.txt`.

---

## Folder structure to upload

```
/
├── index.html
├── robots.txt
├── sitemap.xml
└── images/
    ├── concrete-walkways-dallas-tx-hero.jpg              (1600×900)
    ├── concrete-walkway-dallas-clay-soil-base.jpg        (1200×900)
    └── stamped-concrete-walkway-dallas-tx-garden-path.jpg (1200×900)
```

Create the `images/` folder and drop in three photos using exactly those filenames
(keyword-rich filenames are part of the on-page SEO). Until the photos are added,
the page shows a clean dark placeholder instead of a broken image icon — nothing breaks.

Recommended: save as WebP or compressed JPEG under 250 KB each.

---

## Before going live — edit these

1. **Domain** — replace `https://concretepaversdallastx.com/` everywhere:
   - `<link rel="canonical">` and the Open Graph URL in `index.html`
   - the JSON-LD block at the bottom of `index.html`
   - `robots.txt` (Sitemap line)
   - `sitemap.xml` (all `<loc>` entries)
2. **Business name** — currently "Concrete Pavers Dallas TX" in the header, footer and schema.
3. **Service areas** — edit the tag list in the `#areas` section to match where you actually work.
4. **`lastmod`** in `sitemap.xml` — update whenever you change the page.

---

## SEO already built in

- **H1:** Concrete Walkways Dallas TX (used once)
- Keyword and natural variants ("concrete walkway", "poured concrete path", "Dallas TX")
  placed in title, meta description, H1, first paragraph, H2s, image alt text and filenames
- Semantic heading hierarchy: H1 → H2 → H3, no skipped levels
- ~1,400 words of original, non-duplicated body copy
- Structured data: `WebPage` + `Service` + `FAQPage` (FAQ schema matches the on-page FAQ exactly, as Google requires)
- Open Graph + Twitter card tags
- `loading="lazy"` on below-fold images, `eager` on the hero
- Explicit `width`/`height` on images to prevent layout shift (CLS)
- Descriptive internal anchors in the nav and footer

## Outbound link

There is exactly **one** outbound link on the page, placed in the **second paragraph** of the intro section:

```html
<a href="https://estradafencing.com/concrete-dallas-tx/">Discover More</a>
```

It sits inside a contextually relevant sentence about wider Dallas concrete services, so it reads
naturally and passes topical relevance. It is `dofollow` (no `rel="nofollow"` attribute).
There are no other external links anywhere in the file — check before adding any.

## Deliberately not included

- No phone number
- No call button / click-to-call
- No contact form

---

## Design

- **Theme:** dark grey, solid (no gradient washes) — `#1b1d1e` base, `#232628` alternating sections, `#2b2f31` raised surfaces
- **Accent:** muted bronze `#c2924f`, used only on rules, markers and links
- **Type:** Marcellus (display serif, luxury feel) + Inter (body), loaded from Google Fonts
- **Animation:** hero entrance sequence on load, scroll-reveal on each section, animated step rail,
  underline sweep on finish cards, image de-saturation on hover, animated FAQ accordion
- **Accessibility:** visible keyboard focus rings, `prefers-reduced-motion` fully respected (all motion disabled)
- **Responsive:** grids collapse to single column under 900px; tested down to 360px

---

## After upload

1. Verify `https://yourdomain.com/robots.txt` and `/sitemap.xml` load in a browser.
2. Submit the sitemap in Google Search Console → Sitemaps.
3. Run the page through the Rich Results Test to confirm the FAQ schema is valid.
4. Request indexing for the homepage URL.
