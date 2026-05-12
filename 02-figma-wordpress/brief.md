# 02 — Figma Design + WordPress Integration

## What you will deliver

A single landing-page section for a fictional brand, designed in Figma and implemented as a published WordPress page on a host of your choice.

You will submit, in `02-figma-wordpress/submission/`:

1. **`design.fig`** — your raw Figma file (NOT a PNG / PDF / JPG export). See the "Submitting your Figma file" section below for how to export `.fig` from the Figma desktop app, and the fallback if the file is too large for git.
2. **`PUBLISHED-URL.md`** — a single line containing the live URL of your published page.
3. **`notes.md`** *(optional but recommended)* — which host you used, which plugins you installed, and any deviations between your design and the live page (with reasons).

***

## The brand

You are designing for **Atlas Coffee Tangier** — a fictional small specialty coffee shop in Tangier.

The brand kit is in [`brand-kit/`](./brand-kit/). It contains:

* [`logo.svg`](./brand-kit/logo.svg) — the brand mark
* [`colors.md`](./brand-kit/colors.md) — the 3-color palette with hex codes
* [`typography.md`](./brand-kit/typography.md) — the heading + body fonts (Google Fonts) and usage rules
* [`content.md`](./brand-kit/content.md) — sample copy: headlines, sub-headlines, body paragraph, and CTAs you may use

**Use the brand kit faithfully.** Do not swap fonts. Do not pick "close enough" colors. Do not invent a different logo. Brand fidelity is one of the four scoring dimensions.

***

## What to design

A single landing-page section that contains, in this order, top to bottom:

1. **Hero** — brand logo, big headline, sub-headline, primary CTA, and one image (you may use a free stock photo from Unsplash / Pexels — credit it in `notes.md`).
2. **3-feature block** — three small cards, each with an icon (or simple shape), a short title, and one sentence of body copy. Use the feature copy from `content.md`.
3. **Closing CTA band** — a wide horizontal band with one strong CTA inviting the visitor to take action.

That is the entire page. We do not want a 12-section landing page; we want a clean, well-executed three-section page.

***

## What to do

### Step 1 — Design in Figma

* Create a new Figma file. Name it `Atlas Coffee Tangier - <your-name>`.
* Design at desktop width (1440 px) AND a mobile frame (375 px). Both responsive variants are required.
* Use the colors and fonts from `brand-kit/`. No exceptions.
* Use auto-layout where it makes sense — we will look for it.
* Group / name your layers like an adult, not like `Frame 47`, `Group 219`.

### Step 2 — Set up WordPress

You host this yourself, on a free host of your choice. Some options that are known to work for this test:

* **InfinityFree** (free PHP + MySQL hosting; allows plugin uploads on free tier)
* **000webhost** (similar to InfinityFree)
* **Hostinger** (paid; has a free trial period long enough for this test)
* **Local by Flywheel + Cloudflare Tunnel** (run WordPress locally and expose it through a free Cloudflare Tunnel — no hosting bill, but the page must remain reachable for the duration of our review)

You may use **any** other approach you like, as long as the result is **a real WordPress install serving a real page over HTTPS**, reachable from the public internet. Static HTML files exported from Figma are NOT acceptable.

### Step 3 — Build the page in WordPress

* Use the block editor (Gutenberg) and / or any free page-builder plugin. Elementor's free version is fine. Hand-coded HTML/CSS in a Custom HTML block is also fine. Use whatever lets you reproduce the Figma design well.
* Match your Figma design within \~10% on font sizes, colors, spacing, and proportions.
* The page must be responsive (works on mobile and desktop).
* The page must be published (publicly reachable, not draft, not password-protected).

### Step 4 — Submit

Place files in `02-figma-wordpress/submission/`:

* `design.fig` — see "Submitting your Figma file" below
* `PUBLISHED-URL.md` — a single-line file like:
  ```
  https://atlas-coffee-test.example-host.com/specialty-blend
  ```
* `notes.md` — optional, but recommended if anything about your setup is non-obvious

***

## Acceptance criteria

| Criterion                                                        | Why it matters                                                  |
| ---------------------------------------------------------------- | --------------------------------------------------------------- |
| Page loads in under \~4 seconds on simulated 4G                  | Real users will leave a slow page                               |
| Renders correctly on mobile and desktop                          | The job is mobile-first                                         |
| Hero, feature block, and CTA match the Figma within \~10%        | Tests integration accuracy                                      |
| Brand colors and fonts respected (no random Tailwind defaults)   | Tests brand fidelity                                            |
| HTTPS works                                                      | Most free hosts give this for free; an HTTP-only page is a fail |
| No visible Lorem Ipsum, no placeholder images, no console errors | Quality-of-finishing signal                                     |

***

## Submitting your Figma file

We want the **raw** **`.fig`** **file**, not an exported PNG / PDF / JPG.

To export `.fig` from the Figma desktop app:

1. Open your file in the **Figma desktop app** (this option is not available in the browser version).
2. Top-left menu -> **File** -> **Save local copy...**
3. Save the resulting `.fig` file into `02-figma-wordpress/submission/` and rename it to `design.fig`.
4. Commit and push.

**If the file is too large for git** (over 100 MB — git will warn you):

* Do NOT commit the file.
* Instead, in `notes.md`, write a section called **"Figma file"** with a public Figma view link (in Figma: Share -> "Anyone with the link" can view -> copy link).
* Explain in one sentence why you chose the link route (file size).

This fallback is allowed and not penalized. It is just so we don't hit GitHub's file-size limits.

***

## What we're grading (35 points total)

| What                                                 | \~Points |
| ---------------------------------------------------- | -------- |
| Design quality (hierarchy, balance, typography, CTA) | \~10     |
| Brand fidelity (colors, fonts, tone)                 | \~9      |
| Integration accuracy (live page vs Figma)            | \~10     |
| Site setup (loads, responsive, HTTPS, no errors)     | \~6      |

The detailed sub-rubric is internal. See [`CONTRIBUTING.md`](../CONTRIBUTING.md) for the public scoring overview.
