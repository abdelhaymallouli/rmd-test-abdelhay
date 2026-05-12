# CONTRIBUTING — How your work will be graded

This document tells you, in plain terms, how RMD will grade each section of this test. Read it before you start so you know where to spend your effort.

We do **not** publish the auto-grader answer key or the detailed sub-rubrics — but the section-level allocation below is the truth, and it is not negotiable.

---

## Total: 100 points

| Section                           | Points | Grading        |
| --------------------------------- | ------ | -------------- |
| 1. Multiple-choice quiz (QCM)     | 25     | Auto-graded    |
| 2. Figma design + WordPress       | 35     | Manual review  |
| 3. SEO audit                      | 20     | Manual review  |
| 4. AI + automations               | 20     | Manual review  |

**Bands:**
- **75-100** — Strong; fast-track to interview.
- **60-74** — Invite to interview.
- **50-59** — Borderline; depends on the rest of the cohort.
- **Below 50** — Not moving forward.

---

## Section 1 — QCM (25 points, auto-graded)

- 25 questions (mix of WordPress, on-page SEO, off-page SEO, technical SEO, AI tool literacy).
- 1 point per question. No partial credit on multi-select questions — your selected set must match exactly.
- Submit by editing `01-qcm/answers.json`. Do **not** edit `01-qcm/questions.md`.

We grade by running an internal Python script that compares your `answers.json` to the canonical answer key. Quick to run, deterministic, no human discretion.

---

## Section 2 — Figma design + WordPress integration (35 points)

Manually reviewed. We look at four things:

- **Design quality (~10 pts).** Is the section actually well-designed? Visual hierarchy, balance, typography choices, use of whitespace, tasteful CTA.
- **Brand fidelity (~9 pts).** Did you respect the colors, fonts, and tone in the brand kit? Or did you ship random Tailwind defaults?
- **Integration accuracy (~10 pts).** Does the live page match the Figma file in spacing, sizes, and proportions? Within ~10% tolerance is fine; obvious deviations cost points.
- **Site setup (~6 pts).** Does the page actually load? Mobile-responsive? HTTPS? No broken images or 404s?

Bonus / penalty signals:
- Bonus for: clean URL slugs, proper page title, Open Graph tags set, sensible alt text on images.
- Penalty for: visible Lorem Ipsum, broken responsiveness, missing favicon, console errors visible to a normal visitor.

---

## Section 3 — SEO audit (20 points)

Manually reviewed.

- **Coverage (~7 pts).** Did you cover all three SEO dimensions — on-page, technical, off-page — with real findings, not just lists?
- **Tool fluency (~5 pts).** Did you actually use the recommended free tools (Lighthouse, PageSpeed Insights, Rank Math, Search Console, Ahrefs Webmaster Tools)? Show the data, not just opinions.
- **Quality of recommendations (~6 pts).** For each issue: severity rating + recommended fix. Vague advice ("improve content") loses points; specific advice ("rewrite the H1 from 'Welcome' to a keyword-led 'Specialty Coffee in Tangier - Atlas Coffee'") earns them.
- **Off-page realism (~2 pts).** Your page is brand new — it has zero backlinks. We want you to acknowledge that and propose a realistic 90-day backlink-building plan, not pretend.

---

## Section 4 — AI + automations (20 points)

Manually reviewed across three parts:

- **Part A — practical AI prompt task (~8 pts).** Quality of your prompt(s). Quality of the AI output. Quality of your editorial judgment in picking the winning variation. Are the meta-descriptions actually within 150-160 characters? Is the keyword placed naturally?
- **Part B — automation sketch (~8 pts).** Tool choice with justification, clear trigger, clear steps, real failure-mode awareness, a readable diagram (mermaid or ASCII). We are not testing you on the *exact* tool you pick — we are testing whether you can think in terms of triggers, steps, and what could break.
- **Part C — open thinking (~4 pts).** Did you spot a genuinely repetitive agency task and propose a sane automation, in 5 lines? We reward concrete examples ("auto-generate weekly client status emails from ClickUp tasks") over abstract ones ("automate communication").

---

## What we are NOT grading you on

- Your English perfection. We want clear, not literary. Typos do not cost points unless they make a section unreadable.
- Whether you used ChatGPT, Claude, Gemini, or anything else. Use what you want — but tell us what you used and why.
- The visual prettiness of your repo's README. Filling in the asked-for files in the right places is enough.

---

## What disqualifies a submission

- Repo is private.
- Sections submitted blank.
- Plagiarism from another candidate's public repo.
- Submitted after the deadline without prior notice.
- The "WordPress page" is just a Figma export saved as an HTML file. We test that the URL serves real WordPress.

---

## Questions?

Email the address in your invitation. We answer questions about briefs and process. We do not give hints on answers.
