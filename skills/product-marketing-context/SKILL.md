---
name: product-marketing-context
description: "Builds the product positioning document — customer language, differentiation, personas, and proof points. Triggers for 'positioning', 'target audience', 'differentiation', 'proof points', 'customer language', or 'product marketing context'."
---

# Product Marketing Context Builder

You build and maintain `product-marketing-context.md` — the deep positioning reference for a brand. Every marketing specialist reads this before creating any content, ad, email, or campaign. It captures the exact customer language, objections, differentiation, and proof points that make marketing feel native rather than generic.

The document lives at `./brands/{brand-slug}/product-marketing-context.md`. It complements (not replaces) `brand-context.md` — that's the lightweight onboarding doc; this is the strategic intelligence layer.

## Starting Context Router

Before building or updating this document, quickly identify the strongest context the user is starting from:

- **Blank page / new brand** — use a focused interview to surface positioning, audience, objections, and proof without pretending the strategy is already defined.
- **Existing repo, docs, brand materials, or internal assets** — treat those sources as evidence of the current product and messaging, then translate what matters into sharper market context rather than implementation advice.
- **Live URL or public presence** — use the public site, pages, and visible messaging as inputs for positioning analysis, gap-finding, and clarification of what the market currently sees.

If some sources are missing, continue with the best available context instead of blocking progress. In all cases, stay at the product-marketing context layer: clarify strategy, language, differentiation, and customer reality so downstream specialists can execute better.

---

## 0. Brand Selection

Before anything else:

1. Check if a brand is already active in the conversation context.
2. If not, scan `./brands/` for existing brand directories.
3. If multiple brands exist, present a numbered selection menu.
4. Once selected, read `./brands/{brand-slug}/brand-context.md`.

Never operate without knowing which brand you're working on.

---

## 1. Check What Already Exists

### Step 1 — Existing product marketing context?

Look for `./brands/{brand-slug}/product-marketing-context.md`.

- **If found**: Read it. Present: "Your product marketing context was last updated {date}. What would you like to update — or should I review it for gaps and suggest additions?"
- **If not found**: Proceed to Step 2.

### Step 2 — SOSTAC files available?

Scan `./brands/{brand-slug}/sostac/` for completed phase files:

| SOSTAC File | Rich content to extract |
|---|---|
| `01-situation.md` | Competitive landscape, SWOT, customer language from reviews, market context |
| `02-objectives.md` | Goals, target metrics, success definition |
| `03-strategy.md` | Target segments, personas, positioning, differentiation, value proposition |
| `04-tactics.md` | Objections addressed in channel strategy, proof points referenced |

- **If SOSTAC files exist** → go to **Mode A: Auto-Extract** (Section 2)
- **If no SOSTAC files** → go to **Mode B: Focused Interview** (Section 3)

---

## 2. Mode A: Auto-Extract from SOSTAC

When SOSTAC files exist, extract rather than re-ask. The user already answered these questions in depth — respect that.

### Process

1. Read all available SOSTAC phase files in full.
2. Map their content to the 12 sections of `product-marketing-context.md` (Section 4 template).
3. Identify gaps — what SOSTAC doesn't cover well (typically: verbatim customer language, specific objections word-for-word, concrete proof point numbers).
4. Show the user what you have and what you still need:

```
I've extracted the following from your SOSTAC plan:

✓ Product overview (Situation Analysis)
✓ Target audience + 2 personas (Strategy)
✓ Competitive landscape — 4 competitors mapped (Situation Analysis)
✓ Differentiation and positioning statement (Strategy)
✗ Customer language — need verbatim phrases your customers actually use
✗ Objections — partially covered, need exact wording and responses
✗ Proof points — need specific numbers and case study results

I have 4 focused questions to fill these gaps. Ready?
```

5. Ask only for what's genuinely missing. Never re-ask what SOSTAC already answered.

---

## 3. Mode B: Focused Interview (No SOSTAC)

When no SOSTAC files exist, gather context through a tight 3-round interview. 3-4 questions per round. Acknowledge answers and probe weak spots before moving on.

### Round 1 — Product and Audience

- What does your product do, in one sentence — using the words your best customers would use?
- Who is your primary buyer? Role, company size or context, what situation are they in when they first go looking?
- What problem were they trying to solve — and what were they doing before they found you?
- Who is your ideal customer — the one who gets the most value and never leaves? What makes them different from a bad-fit customer?

### Round 2 — Market and Differentiation

- Who are your top 2-3 competitors? What do customers think of them?
- Why do customers choose you over the alternatives? What's the real reason, beyond the marketing message?
- What objections do you hear most before someone decides to buy? What are the exact words they use?
- Who should you turn away — who is genuinely a bad fit?

### Round 3 — Language and Proof

- What specific phrases or words do your customers use to describe their problem? Exact language from reviews, sales calls, support tickets — not paraphrased.
- What concrete results do your best customers achieve? Numbers, timeframes, before/after comparisons.
- How do you want your brand to sound? Pick 3 adjectives, and tell me one thing you never want to sound like.
- What are your primary marketing goals for the next 6-12 months?

Probe vague answers. "What does that look like specifically?" and "Can you give me an example?" are your best tools. Section 9 (Customer Language) should contain verbatim quotes — don't let the user paraphrase when they might have the real words available.

---

## 4. Document Template

> **Template:** See `./references/document-template.md` for the full 12-section product marketing context template. Save the completed document to `./brands/{brand-slug}/product-marketing-context.md`.

---

## 5. After Writing

1. **Summarize what was captured** — sections completed, anything marked incomplete, what would strengthen it (e.g., "Section 9 only has 2 customer quotes — the more verbatim phrases you can add over time, the better every campaign gets").

2. **Sync with brand-context.md** — if anything in `product-marketing-context.md` expands or contradicts `brand-context.md`, update `brand-context.md` to stay consistent. They should agree, not diverge.

3. **Tell the user how this gets used:**

```
Saved to:
./brands/{brand-slug}/product-marketing-context.md

Every marketing specialist — content, email, SEO, paid ads, social —
will read this before any task for {Brand Name}. The Customer Language
section (§9) is especially powerful for copywriting: those verbatim
phrases outperform anything we could write from scratch.

Keep it current: update Section 11 whenever you get a strong
testimonial, and Section 9 whenever you hear a customer phrase that
just works. Fresh context = better output from every specialist.
```

4. **Recommend the next step:**
   - No SOSTAC plan yet → "Want to run a full SOSTAC plan to build your complete marketing strategy?"
   - SOSTAC complete, not implementing → "Context is set — ready to start implementation?"
   - Already implementing → "Refresh this quarterly as you gather new customer data and proof points."

---

## 6. Updating the Document

When the user asks to refresh or update:

1. Read the current `product-marketing-context.md`.
2. Ask what's changed: new competitors, fresh customer feedback, updated positioning, new proof points, revised goals?
3. Edit only the relevant sections — don't regenerate the whole document.
4. Update the "Last updated" date.
5. If changes are significant (new positioning, new primary persona), note a brief changelog at the top of the file.


---

## Output Contract

Product marketing context deliverables include:
- **Positioning statement**: clear articulation of who, what, why, and how
- **Target personas**: detailed profiles with goals, pain points, and language
- **Differentiation**: competitive advantages with proof points
- **Customer language**: actual phrases and terms the audience uses
- **Messaging framework**: hierarchy of messages by persona and funnel stage
