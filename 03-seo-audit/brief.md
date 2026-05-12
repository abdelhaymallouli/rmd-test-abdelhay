# 03 — SEO Audit

## What you will deliver

A structured SEO audit of **the WordPress page you published in Section 2**. Submit it as `03-seo-audit/submission/audit.md`.

The audit must cover all three SEO dimensions — **on-page**, **technical**, and **off-page** — and end with a concrete, prioritized action plan.

Length expectation: **~800 words minimum**. Quality and specificity matter more than length, but if your audit is shorter than 800 words you have probably skipped something.

---

## Why we are asking for this

Auditing your own freshly published page tells us four things at once:

1. Whether you understand all three SEO dimensions and what each one actually means.
2. Whether you know how to use the standard free tools.
3. Whether you can read a Lighthouse / PageSpeed / Search Console report and turn raw numbers into actions.
4. Whether you are honest about your own work — many candidates over-claim on their own pages, and we notice.

---

## Tools to use (all free)

| Tool                              | What you use it for                                                                  |
| --------------------------------- | ------------------------------------------------------------------------------------ |
| **Lighthouse** (Chrome DevTools)  | Performance, Accessibility, Best Practices, SEO scores                               |
| **PageSpeed Insights**            | https://pagespeed.web.dev — Core Web Vitals (LCP, INP, CLS) on real-device profiles  |
| **Rank Math** (free WP plugin)    | On-page checks for your published page (title, meta, H1, alt, schema, etc.)         |
| **Google Search Console**         | Verify the property if you can; check indexability, sitemap submission              |
| **Ahrefs Webmaster Tools** (free) | https://ahrefs.com/webmaster-tools — backlinks, organic keywords, site issues       |
| Browser dev tools                 | Inspect HTML to verify title tag, meta description, schema markup                    |

You are not required to use *all* of these — but every claim you make in the audit must be backed by output from one of them.

---

## Required structure for `audit.md`

Use this skeleton. You may add sub-sections, but do not skip any of the headings below.

```markdown
# SEO Audit — [your published URL]

**Audited on:** YYYY-MM-DD
**Audited by:** <your name>
**Tools used:** [list]

## 1. Page snapshot
- URL:
- Page title (as currently shown in the SERP / browser tab):
- Meta description:
- Primary keyword you optimized for:
- Word count of main content:

## 2. On-page SEO
- Title tag — length, keyword placement, judgment
- Meta description — length, hook, judgment
- H1 / H2 hierarchy — what is on the page, is it correct?
- Image alt text — present? meaningful?
- Internal links — how many, where they go
- Content quality — is the page actually about something useful?

## 3. Technical SEO
- Is the page indexable? (check meta robots, robots.txt, sitemap)
- Is there an XML sitemap? Is the page in it?
- Schema markup — what is present? what should be present?
- Core Web Vitals — LCP, INP, CLS (give the actual numbers from PageSpeed Insights)
- Mobile-friendly? (Lighthouse mobile audit)
- HTTPS? Mixed content?
- Any other issues Lighthouse / PageSpeed flagged

## 4. Off-page SEO
- Backlink profile (almost certainly zero — that is fine, acknowledge it)
- A realistic 90-day backlink-building plan (3-6 specific, actionable tactics, not "build great content and they will come")

## 5. Issues table — prioritized
| Severity (high / med / low) | Issue                                          | Recommended fix                                       |
| --------------------------- | ---------------------------------------------- | ----------------------------------------------------- |
| high                        | Example: meta description is 240 chars (truncated) | Rewrite to 150-160 chars including the keyword "X"     |
| ...                         | ...                                            | ...                                                   |

## 6. Top 3 things to fix this week
1. [most important fix, with the exact step]
2. [second]
3. [third]
```

---

## What good looks like

- **Specific over vague.** "Improve content" is useless. "Add a 200-word section about espresso preparation, targeting the keyword 'specialty espresso tangier' as an exact-match phrase in the H2" is useful.
- **Numbers, not adjectives.** "LCP is 4.7 s on mobile (PageSpeed, Moto G4 profile, 4G)" beats "LCP is slow."
- **Honest, not defensive.** It is your own page, but we are grading the audit, not the page. Catching your own issues earns points; hiding them costs them.

## What we are grading (20 points total)

| What                                                                          | ~Points |
| ----------------------------------------------------------------------------- | ------- |
| Coverage — all three dimensions, with real findings                           | ~7      |
| Tool fluency — actually using the recommended free tools, showing the data    | ~5      |
| Quality of recommendations — specific, prioritized, actionable                | ~6      |
| Off-page realism — acknowledges zero backlinks, proposes a real 90-day plan   | ~2      |

## What disqualifies the audit

- Auditing a different page than the one you submitted in Section 2.
- Claiming a Core Web Vitals number with no screenshot or data source.
- Writing an audit for a page that is not actually live at review time.
