# 04 — AI + Automations

## What you will deliver

This section has three small parts. Total expected output: about **600-800 words** across the two submission files.

You will submit, in `04-ai-automations/submission/`:

- **`prompt-task.md`** — Part A
- **`automation-sketch.md`** — Parts B and C (Part C goes at the bottom)

No code execution required. We are grading your thinking, your prompts, your tool choices, and your output quality.

---

## Part A — Practical AI prompt task (~8 / 20 pts)

### Scenario

Atlas Coffee Tangier (the fictional brand from Section 2) wants a new product page for their signature blend. You need to give them **3 H1 + meta-description variations** for that product page.

### Constraints

- Target keyword: **"specialty coffee tangier"**.
- Each H1 must read like a real H1 (not a meta-tag-ish phrase). Around 50-65 characters is a good range.
- Each meta description must be **150-160 characters maximum**. Anything longer gets truncated in Google's results.
- The keyword should appear naturally in at least the H1 of each variation, ideally in the meta too.
- Do not output 3 near-identical variations. They should be meaningfully different (different angles: provenance, craft, location, etc.).

### Use any AI you want

Claude, ChatGPT, Gemini, Mistral, anything. Free tier is fine.

### Submit, in `prompt-task.md`

```markdown
# Part A — Prompt task

## AI tool used
[Name + version, e.g. "ChatGPT, GPT-4o, free tier" or "Claude, Sonnet 4.6, free tier"]

## Why I picked this tool
[2 lines max]

## Prompt(s) I used
> [paste your full prompt here, in a quote block, exactly as you sent it]

(If you iterated, paste the final version of your prompt that produced the output you submit. Optionally include a one-line note about what you changed and why.)

## Raw output from the AI (all 3 variations, unedited)
1. **H1:** ...
   **Meta:** ...
2. **H1:** ...
   **Meta:** ...
3. **H1:** ...
   **Meta:** ...

## Final pick + 2-line justification
**Picked variation: #X**
[2 lines explaining why — what makes it the best one for SEO and for the brand voice]
```

### What we judge

- Quality of your prompt (specific, with constraints, with the brand context).
- Quality of the AI output (do the 3 variations actually meet the constraints?).
- Quality of your editorial judgment when you pick the winner.

---

## Part B — Automation sketch (~8 / 20 pts)

### Scenario

A WordPress site (any site, doesn't have to be related to Atlas Coffee) publishes a new blog post. **You want a short summary of that post posted automatically to a Slack channel** so the whole team sees it.

### Constraint

You must use a **no-code or low-code tool**. Any of these is fine:
- **n8n** (self-hosted or cloud)
- **Make** (formerly Integromat)
- **Zapier**
- **GitHub Actions** (yes, GitHub Actions counts)
- **WordPress webhooks** (built-in or via a plugin like WP Webhooks)

### Submit, in `automation-sketch.md`

```markdown
# Part B — Automation sketch

## The goal in one sentence
[Plain English, one sentence.]

## Tool I picked + 2-line justification
[Tool name. Why this one over the others — pick a real reason, not "because I know it".]

## Trigger
[What kicks off the automation. Be specific — webhook URL? RSS feed? Cron poll every N minutes?]

## Steps (numbered)
1. ...
2. ...
3. ...
4. (etc.)

## 2 failure modes I would handle
1. **Failure:** [what could break]
   **Handling:** [what the automation does about it — retry? alert? skip?]
2. **Failure:** [...]
   **Handling:** [...]

## Diagram
[Insert a diagram — either a mermaid code block or ASCII art. Whichever is clearer.]

## (Part C continues below)
```

### What we judge

- Real understanding of *trigger -> processing -> output*.
- Tool choice with a real reason.
- Failure-mode awareness (this is the part most candidates skip).
- A readable diagram — clarity beats prettiness.

---

## Part C — Open thinking (~4 / 20 pts)

Append this section at the bottom of `automation-sketch.md`:

```markdown
## Part C — A repetitive task I would automate

[Pick ONE repetitive task that exists in a real marketing-agency workflow. Describe in 5 lines:
- What the task is
- Why it is repetitive (frequency, who does it today)
- Which tool you would use to automate it
- The trigger and the action, in one sentence
- The biggest failure mode]
```

### What we judge

- Did you pick a *real* repetitive agency task (e.g. "compile weekly client status emails from ClickUp tasks") rather than something generic ("automate communication")?
- Is your sketch concrete and plausible?

---

## What disqualifies this section

- Fabricated AI output (we can tell).
- Empty `prompt-task.md` or `automation-sketch.md`.
- Submitting 3 variations in Part A that are obvious paraphrases of each other.

---

## Total points for this section: 20

| Part                                | ~Points |
| ----------------------------------- | ------- |
| A — practical AI prompt task        | ~8      |
| B — automation sketch               | ~8      |
| C — open thinking                   | ~4      |
