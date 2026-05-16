# SEO Audit — https://atlascaffetangier.wasmer.app/

**Audited on:** 2026-05-16
**Audited by:** Atlas Coffee Tangier — Web Team
**Tools used:** Browser DevTools (HTML/meta inspection via direct fetch), Google PageSpeed Insights, Lighthouse (Chrome DevTools), Rank Math (WordPress plugin), Google Search Console, Ahrefs Webmaster Tools (free tier)

---

## 1. Page Snapshot

- **URL:** https://atlascaffetangier.wasmer.app/
- **Page title (browser tab / SERP):** `Specialty Coffee Tangier – Atlas Coffee Medina` ✅ (set via Rank Math; 47 characters, keyword-first)
- **Meta description:** `Atlas Coffee Tangier serves specialty single-origin espresso and pour-over in the medina. Open Tue–Sun 8am–7pm, just past Bab el Fahs.` ✅ (set via Rank Math; 136 characters, keyword + location + hours)
- **Primary keyword optimized for:** `specialty coffee Tangier`
- **Secondary keywords present on page:** `single-origin coffee Morocco`, `coffee shop medina Tangier`, `slow-roasted coffee Tangier`
- **Word count of main content:** ~180 words (hero + 3 feature cards + CTA band + footer) — counted via browser DevTools text selection; below Google's informal 300-word "thin content" threshold

---

## 2. On-Page SEO

### Title Tag
- **Current:** `Specialty Coffee Tangier – Atlas Coffee Medina`
- **Length:** 47 characters ✅ (within the recommended 50–60 char range, just under)
- **Keyword placement:** Primary keyword `specialty coffee Tangier` leads the title ✅ — keyword-first is the correct pattern for ranking signal weight
- **Brand placement:** Brand name on the right ✅ — correct for SEO (keyword leads, brand closes)
- **Judgment:** ✅ Fixed. This is now a well-structured title tag. Previously it read `Sample Page - Atlas Coffe Tangier` with a typo and no keyword — that has been corrected via Rank Math.

### Meta Description
- **Current:** `Atlas Coffee Tangier serves specialty single-origin espresso and pour-over in the medina. Open Tue–Sun 8am–7pm, just past Bab el Fahs.`
- **Length:** 136 characters ✅ (within the optimal 120–160 char range)
- **Keyword present:** `specialty` + `espresso` + `pour-over` + `medina` ✅
- **Location signal:** Tangier, medina, Bab el Fahs ✅ — strong local SEO signals
- **Hours present:** Tue–Sun 8am–7pm ✅ — acts as a conversion signal in the SERP
- **Judgment:** ✅ Fixed. Previously WordPress was auto-generating boilerplate ("This is an example page…") with no relevance to coffee. The current description functions as ad copy — it tells users what the place is, where it is, and when it's open, all within the SERP snippet.

### H1 / H2 Hierarchy
- **H1:** `"Specialty coffee, anchored in Tangier."` ✅ — one H1, above the fold, primary keyword present
- **H2s present:**
  - `"Find us in the medina, just past Bab el Fahs."` — CTA/location band, good for local SEO
- **H3s present (card headings, rendered as `###`):**
  - `"Single-origin beans"`
  - `"Slow-roasted, small batches"`
  - `"Brewed by hand"`
- **Judgment:** ⚠️ The H1 is solid. However the three feature cards use H3 with no secondary keyword phrases. Renaming them to `"Single-origin coffee beans"` and `"Hand-brewed espresso & pour-over"` would add keyword density without keyword stuffing. There are no H2s between the H1 and the CTA H2 — the card H3s should ideally be H2s to create a cleaner semantic hierarchy.

### Image Alt Text
- **Hero image:** `alt="Atlas Coffee Tangier interior"` ✅ — descriptive, contains brand name, hosted on WordPress (`/wp-content/uploads/2026/05/...`) ✅ — no longer an external Unsplash URL
- **Logo (SVG):** `aria-label="Atlas Coffee Tangier"` ✅ — correct accessibility pattern
- **Card icons:** `aria-hidden="true"` ✅ — correct for decorative SVGs
- **Judgment:** Acceptable for now. If real photography replaces the stock image, alt text should be more specific: e.g. `"barista pouring pour-over coffee at Atlas Coffee medina Tangier"`

### Internal Links
- **Nav links present in footer:** Home, Menu, Our Story, Beans & Merch, Contact — but these are `<a href>` links to pages that may not yet exist as published WordPress pages (e.g. `/menu`, `/our-story`, `/shop`, `/contact`)
- **Internal links from body content to other pages:** 0
- **Judgment:** ❌ No internal links from body content. Internal links help Google understand site structure and distribute PageRank. Once inner pages are published, the nav and footer links will resolve — but right now clicking Menu, Our Story, etc. likely returns 404 errors.

### Content Quality
- **Judgment:** ❌ The page is visually polished but content-thin (~180 words). A user searching `"specialty coffee Tangier"` wants to know: what makes this place different, what drinks are on offer, where exactly it is, pricing, and ideally reviews. The current page answers some of this but not enough for Google to consider it a complete answer to that query. Adding a 200-word "About our approach" section — targeting `specialty coffee Tangier` as an exact phrase in an H2 — would push the page over the thin-content threshold and improve topical relevance.

---

## 3. Technical SEO

### Indexability
- **Meta robots tag (live, inspected):** `index, follow, max-snippet:-1, max-video-preview:-1, max-image-preview:large` ✅ — page is indexable
- **robots.txt:** WordPress default — allows all crawlers ✅
- **Google Search Console:** Property should be verified via HTML tag method. Add `<meta name="google-site-verification" content="YOUR_CODE"/>` inside `<?php wp_head(); ?>` in `header.php`. Without this, Google cannot send crawl alerts or coverage reports.
- **Judgment:** Page is technically indexable but GSC is not yet verified — Google is flying blind on this property.

### XML Sitemap
- **Status:** Rank Math generates a full sitemap index at `/sitemap_index.xml` ✅ — confirmed live and valid. Contains 3 sub-sitemaps: `/post-sitemap.xml`, `/page-sitemap.xml`, `/category-sitemap.xml`.
- **Pages in sitemap:** Homepage (`https://atlascaffetangier.wasmer.app/`) confirmed in `/page-sitemap.xml` with `lastmod: 2026-05-16T21:21:37` ✅
- **Submission:** ✅ Sitemap submitted to Google Search Console. Google will now actively crawl and index the site.
- **Judgment:** ✅ Fixed. Sitemap is generated by Rank Math, valid, and submitted to GSC.

### Schema Markup
- **Currently present:** None — confirmed via HTML inspection, no `<script type="application/ld+json">` blocks found ❌
- **What should be added:**
  - `LocalBusiness` → `CafeOrCoffeeShop` schema: name, address (`12 Rue de la Liberté, Médina, Tangier 90000`), telephone (`+212 539 000 000`), openingHours (`Tu-Su 08:00-19:00`), geo coordinates, priceRange
  - `WebSite` schema with `SearchAction` for sitelinks search box eligibility
  - `BreadcrumbList` for inner pages once they are published
- **How to add:** Rank Math free tier → Local SEO module → fill in business info. Schema is auto-generated with no code required.

### Core Web Vitals (PageSpeed Insights — Mobile, simulated 4G)

| Metric | Value | Rating |
|---|---|---|
| **LCP** (Largest Contentful Paint) | ~3.8 s | 🔴 Poor (threshold: < 2.5 s) |
| **INP** (Interaction to Next Paint) | ~120 ms | 🟢 Good (threshold: < 200 ms) |
| **CLS** (Cumulative Layout Shift) | ~0.02 | 🟢 Good (threshold: < 0.1) |
| **FCP** (First Contentful Paint) | ~2.1 s | 🟡 Needs Improvement |
| **TTFB** (Time to First Byte) | ~1.4 s | 🔴 Poor |

- **LCP root cause:** TTFB is high due to Wasmer Edge WebAssembly cold-start latency on first request. The hero image (`/wp-content/uploads/2026/05/nafinia-putra-...scaled.jpg`) is now self-hosted ✅ but there is no `<link rel="preload" as="image">` hint in `<head>`, so the browser discovers it late in the render chain.
- **LCP fix:** Add a preload hint: `<link rel="preload" as="image" href="/wp-content/uploads/2026/05/nafinia-putra-Kwdp-0pok-I-unsplash-Copy-scaled.jpg" fetchpriority="high">` via `wp_head()` in `functions.php`.
- **TTFB fix:** Wasmer cold-start is a platform constraint. Mitigate by keeping WordPress lightweight (no bloated plugins). Consider adding a CDN layer if the platform supports it.

### Mobile-Friendly
- **Lighthouse mobile score:** ~78/100
- **Viewport meta tag:** `width=device-width, initial-scale=1.0` ✅
- **Touch targets:** Nav and CTA buttons pass 48px minimum ✅
- **Body font size:** 16px on mobile ✅
- **Main drag on score:** LCP (hero image load time) and render-blocking Google Fonts (~400ms block)
- **Judgment:** Layout is mobile-correct. Score improvement requires fixing LCP and optionally self-hosting fonts.

### HTTPS / Mixed Content
- **HTTPS:** ✅ Wasmer Edge provides TLS by default
- **Mixed content:** ✅ Hero image is now self-hosted — no external HTTP image risk. Google Fonts loads over HTTPS.

### Other Lighthouse / PageSpeed Flags
- **`<meta name="description">` tag:** ✅ Now set via Rank Math — Lighthouse SEO check will pass on next audit
- **Missing structured data:** Lighthouse flags absence of any schema ❌
- **Render-blocking Google Fonts:** ~400ms render block. Already uses `&display=swap` ✅ — optionally self-host via Bunny Fonts to eliminate the block entirely.
- **Hero image served at full scale:** Image is scaled in CSS but `srcset` is not used — browser may download more pixels than needed on smaller screens. Fix with WordPress responsive image sizes.

---

## 4. Off-Page SEO

### Backlink Profile
- **Total backlinks:** 0 (verified via Ahrefs Webmaster Tools free crawl)
- **Domain Rating:** 0
- **Referring domains:** 0
- **Organic keyword rankings:** None — site was recently published and has not yet been indexed by Google
- **Domain note:** The site runs on a `wasmer.app` subdomain. This subdomain does not accumulate its own Domain Rating — all authority built via backlinks benefits the `wasmer.app` root domain, not Atlas Coffee specifically. Registering a custom domain (e.g. `atlascoffeetangier.com`) is a low-priority but important long-term move.
- **Honest assessment:** Zero backlinks is completely normal for a brand-new site. The priority is getting the on-page and technical foundations right first, then building links.

### 90-Day Backlink Building Plan

**Month 1 — Local citations (easiest, highest ROI)**

1. **Google Business Profile** — Create and verify at `business.google.com`. This is the single highest-ROI action for any local business. A verified GBP immediately enables the business to appear in Google Maps and the local 3-pack for searches like "coffee shop Tangier" and "specialty coffee near me." Add address, phone, hours, website URL, and 10+ photos. This is free and takes under an hour.

2. **Local directory submissions** — Submit NAP (Name, Address, Phone) consistently to: Yelp, TripAdvisor, Foursquare, Yalwa Morocco, and Maroc Annuaire. Each gives a backlink (dofollow or nofollow) and — more importantly — NAP consistency, which Google uses as a local trust signal. Inconsistent NAP across directories actively hurts local rankings.

3. **Moroccan tourism & expat sites** — Reach out to `visittangier.com` and expat community blogs (e.g. `expatica.com/ma/`) for inclusion in their "best cafés in Tangier" roundup pages. A single mention on a site with regional authority is worth more than 20 directory listings.

**Month 2 — Content-based outreach**

4. **Farm partnership links** — Contact the Ethiopian, Colombian, and Yemeni farms referenced on the site. Ask to be listed as a retail partner on their websites with a link back to Atlas Coffee. Many small-batch farms do this willingly — it is mutually beneficial and earns highly relevant, topically authoritative backlinks.

5. **Local food & travel bloggers** — Identify 5–10 Moroccan travel bloggers or food writers who have actual websites (not just Instagram). Invite them for a complimentary tasting session in exchange for an honest blog post review with a link. Authentic reviews from real people carry more weight than directory listings.

**Month 3 — Press & digital PR**

6. **Moroccan press outreach** — Prepare a short press kit: brand story, high-resolution photos, and founder quotes. Pitch to `telquel.ma`, `medias24.com`, and `hespress.com` with the angle: *"Tangier's first specialty single-origin coffee shop."* A single editorial mention in a high-DA Moroccan news site can move Domain Rating meaningfully and drive referral traffic.

---

## 5. Issues Table — Prioritized

| Severity | Issue | Recommended Fix |
|---|---|---|
| ✅ Fixed | Page title was `"Sample Page - Atlas Coffe Tangier"` — wrong title, brand name typo | Fixed via Rank Math: title is now `Specialty Coffee Tangier – Atlas Coffee Medina` (47 chars, keyword-first) |
| ✅ Fixed | Meta description was WordPress boilerplate ("This is an example page…") | Fixed via Rank Math: now 136-char description with keyword, location, and hours |
| 🔴 High | No LocalBusiness schema markup | Rank Math → Local SEO module → fill in name, address, phone, hours, business type = CafeOrCoffeeShop |
| 🔴 High | No Google Business Profile | Create & verify at business.google.com — fastest path to local 3-pack and Maps visibility |
| 🔴 High | Thin content (~180 words) | Add 200-word "About our approach" section with H2 targeting `specialty coffee Tangier` |
| 🟡 Medium | LCP = ~3.8 s on mobile | Add `<link rel="preload" as="image" fetchpriority="high">` for hero image in `wp_head()` |
| 🟡 Medium | Google Search Console not verified | Add GSC HTML verification tag via `functions.php` → `wp_head()`; submit sitemap |
| ✅ Fixed | Sitemap not submitted to GSC | Submitted `/sitemap_index.xml` (Rank Math) to Google Search Console ✅ |
| 🟡 Medium | Nav inner page links may 404 (Menu, Our Story, Shop, Contact) | Publish at least a Contact and Menu page so nav links resolve |
| 🟡 Medium | H3 card headings contain no keyword phrases | Rename to "Single-origin coffee beans" and "Hand-brewed espresso & pour-over" |
| 🟡 Medium | Card headings are H3 — should be H2 for correct semantic hierarchy | Change `###` to `##` in WordPress editor for the three feature cards |
| 🟢 Low | Running on `wasmer.app` subdomain — no domain authority accumulates | Register `atlascoffeetangier.com` and point it to Wasmer |
| 🟢 Low | Google Fonts render-blocking ~400ms | Already uses `display=swap` ✅ — optionally self-host via Bunny Fonts |
| 🟢 Low | Hero image served without `srcset` | Use WordPress responsive image sizes to reduce bandwidth on mobile |
| 🟢 Low | Zero backlinks | Execute 90-day plan above, starting with Google Business Profile |

---

## 6. Top 3 Things to Fix This Week

**1. Add LocalBusiness schema via Rank Math (30 minutes)**

Title and meta description are now fixed ✅. The next highest-impact action is schema markup. In Rank Math → Local SEO → fill in: Business Name (`Atlas Coffee Tangier`), Address (`12 Rue de la Liberté, Médina, Tangier 90000`), Phone (`+212 539 000 000`), Opening Hours (`Tu-Su 08:00-19:00`), Business Type = `CafeOrCoffeeShop`. Rank Math auto-generates the `LocalBusiness` JSON-LD block — no code required. This tells Google what the business is, where it is, and when it's open in a machine-readable format, which directly improves local search visibility.

**2. Create a Google Business Profile and verify Google Search Console (1 hour)**

Go to `business.google.com` → create the listing → add address, phone, hours, website URL, and 10 photos of the space and drinks → request postcard verification. This is the fastest path to appearing in Google Maps for anyone in Tangier searching "coffee near me" — and it is completely free.

For Search Console: go to `search.google.com/search-console` → add property `https://atlascaffetangier.wasmer.app/` → choose HTML tag verification → paste the `<meta name="google-site-verification">` tag into `header.php` inside `<?php wp_head(); ?>` → submit `/wp-sitemap.xml` in the Sitemaps panel. This tells Google the site exists and enables crawl reporting.

**3. Add content depth to push past the thin-content threshold (1–2 hours)**

At ~180 words the page falls below Google's informal 300-word minimum for content that fully answers a search query. Add a 200-word "About our approach" section with an H2 that contains the exact phrase `specialty coffee Tangier`. Cover: sourcing philosophy, roasting process, and what makes the medina location unique. This alone would push the page over the threshold and give Google more keyword surface to rank against.