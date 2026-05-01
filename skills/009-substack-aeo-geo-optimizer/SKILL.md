---
name: substack-aeo-geo-optimizer
description: >
  Optimizes any Substack content for AEO (Answer Engine Optimization) and GEO
  (Generative Engine Optimization) — making it citable by ChatGPT, Perplexity,
  Claude, Gemini, and Google AI Overviews. Use this skill whenever the user
  provides a Substack URL or pastes Substack post content and wants to increase
  AI visibility, get cited by AI search engines, optimize for generative search,
  or asks things like "optimize this for AI search", "make this citable by
  ChatGPT or Perplexity", "GEO optimize this post", "AEO this article",
  "how do I get AI to cite my newsletter", "optimize for AI overviews",
  "make this show up in AI answers". Always trigger this skill when the goal
  is to make a Substack post more visible inside AI-generated answers, not just
  Google rankings. This is separate from SEO metadata optimization.
---

# Substack AEO/GEO Optimizer

Transforms a Substack post (URL or pasted text) into content that AI engines
(ChatGPT, Perplexity, Claude, Gemini, Google AI Overviews) are structurally
likely to cite in their answers.

Built on the CITED framework from Passionfruit's AEO methodology and Princeton
KDD 2024 GEO research showing 30-40% citation lift from structured optimization.

---

## Core insight: why most Substack content never gets cited by AI

AI engines don't cite content at random. They cite content that:
1. Answers a specific question **directly and immediately** (in the first 40-60 words)
2. Contains **verifiable facts** with named sources (not vague claims)
3. Uses **structured, extractable formats** (FAQ, lists, definition blocks)
4. Signals **authority** through author credentials and entity clarity
5. Covers the topic **comprehensively enough** to be the best available answer

Most Substack posts are written for human readers who tolerate narrative buildup.
AI engines are pattern-matching for extraction — they need the answer upfront,
the evidence inline, and the structure explicit.

---

## Step 1 — Read and classify the content

If a URL is provided, fetch and read the full post content.
If text is pasted, read it directly.

Classify the post into one of these query types (this determines optimization priority):

| Query type | Signal | Primary AI citation format |
|---|---|---|
| **Definitional** | "What is X", "X explained" | Definition block (40-60 words), then depth |
| **How-to / Process** | "How to X", numbered steps | Numbered list with clear step verbs |
| **Comparison** | "X vs Y", "best X for Y" | Comparison table, named criteria |
| **Opinion / Contrarian** | "Why X is wrong", "The truth about X" | Named expert quotes, cited data |
| **List / Roundup** | "Best X", "Top Y tools" | Structured list with consistent criteria |
| **Case study / Story** | "How I did X", "My results with Y" | Result-first opening, metrics inline |

---

## Step 2 — Run the CITED audit

Score the existing post on each of the 5 CITED dimensions.
Mark each as ✅ Present / ⚠️ Weak / ❌ Missing.

### C — Context clarity
Does the post make clear **who it's for** and **what specific question it answers**?
- ✅ Present: clear audience, specific question answered in title/intro
- ⚠️ Weak: topic is clear but audience or query angle is vague
- ❌ Missing: post reads as general exploration with no specific answerable question

### I — Intent match
Does the content structure match the **intent** of someone asking this question to an AI?
- ✅ Present: informational → direct answer; comparison → table; how-to → steps
- ⚠️ Weak: intent is right but format doesn't match (e.g., steps buried in paragraphs)
- ❌ Missing: content doesn't answer the query an AI user would actually ask

### T — Truth signals
Does the post contain **verifiable, citable evidence**?
Count: named statistics with source, expert quotes with attribution, specific data points.
- ✅ Present: at least 1 cited stat or data point every 150-200 words
- ⚠️ Weak: some stats present but no sources named, or fewer than 1 per 300 words
- ❌ Missing: all claims are opinion-based, no named sources

### E — Extraction format
Is the content **structurally easy for an AI to lift and cite**?
- ✅ Present: direct-answer intro in 40-60 words, FAQ section, or structured list
- ⚠️ Weak: good content but buried in narrative without extractable structure
- ❌ Missing: wall of text, no headers, no extractable blocks

### D — Differentiation
Does the post contain **at least one thing no other source says** in this way?
Original framework, proprietary data, personal result, counter-intuitive claim.
- ✅ Present: clear unique angle, named framework, or original data
- ⚠️ Weak: good writing but no unique insight AI couldn't find elsewhere
- ❌ Missing: standard take on a standard topic

---

## Step 3 — Produce the AEO/GEO optimization report

Output a structured report with these sections:

### Section 1: CITED Audit Score
```
C — Context clarity:    [✅/⚠️/❌] [1-line explanation]
I — Intent match:       [✅/⚠️/❌] [1-line explanation]
T — Truth signals:      [✅/⚠️/❌] [1-line explanation]
E — Extraction format:  [✅/⚠️/❌] [1-line explanation]
D — Differentiation:    [✅/⚠️/❌] [1-line explanation]

AI Citation Readiness: [LOW / MEDIUM / HIGH]
```

### Section 2: Top 3 AI queries this post could answer
List the 3 most likely questions a user would ask ChatGPT or Perplexity that
this post *should* show up in — but probably doesn't yet.

Format:
```
1. "[Exact query a user would type]"
   → Currently blocked by: [what's missing]

2. "[Exact query a user would type]"
   → Currently blocked by: [what's missing]

3. "[Exact query a user would type]"
   → Currently blocked by: [what's missing]
```

### Section 3: Rewritten opening (the AEO intro block)
The single highest-impact fix. Rewrite the post's opening paragraph as an
**AEO-optimized direct-answer intro** of 40-60 words.

Rules for this block:
- Answers the primary query directly in sentence 1
- Includes the most searchable term naturally
- Contains at least 1 verifiable claim (or flags [ADD STAT: topic] if none available)
- Does NOT start with a question, anecdote, or emotional hook
- Reads as the answer an AI would lift verbatim

Format:
```
ORIGINAL OPENING:
[first 50-80 words of original post]

AEO-OPTIMIZED OPENING (40-60 words):
[rewritten version]

Why this works: [1-line explanation of the structural change]
```

### Section 4: FAQ block for AI citation
Generate 3-5 FAQ entries the post should include to capture question-based queries.
These are the questions people ask AI engines that this post answers (or should answer).

Format:
```
**Q: [Natural language question — how a user would actually ask an AI]**
A: [Direct answer in 2-4 sentences. Specific, not vague. Citable.]

**Q: [Question]**
A: [Answer]
```

Rules:
- Questions must be in natural spoken language, not keyword strings
- Answers must be self-contained (readable without the full post context)
- Each answer should be 40-100 words — long enough to be useful, short enough to extract

### Section 5: Truth signal gaps
List the specific claims in the post that currently lack a named source,
and suggest what type of source would make them citable.

Format:
```
CLAIM: "[quote the unsourced claim]"
→ Source needed: [e.g., "Substack 2024 growth data", "email open rate benchmark study", "your own newsletter analytics"]
→ Why it matters: [why an AI would hesitate to cite this without evidence]
```

If the post has no unsourced claims, say so explicitly — that's a strength.

### Section 6: Structural fixes checklist
Quick wins the creator can implement in 15 minutes:

```
□ Add direct-answer intro (see Section 3 above)
□ Add FAQ block (see Section 4 above)
□ [List any missing headers that would help AI parse sections]
□ [Flag any specific stat that needs a source added]
□ [Note if post needs a comparison table]
□ [Note if URL slug should include primary keyword]
□ [Note if post's first 150 words bury the main point]
```

Only include fixes that apply to this specific post. Skip items that are already done.

### Section 7: Platform-specific citation notes
Brief note on which AI engine this post is most likely to get cited by, and why:

```
Most likely platform: [ChatGPT / Perplexity / Google AI Overviews / Claude]
Reason: [1-2 sentences on why this content fits that platform's citation pattern]

Hardest platform to crack: [platform]
What's missing: [specific gap for that platform]
```

Platform citation patterns (reference only — don't show this to user):
- **Perplexity**: favors recent, structured, evidence-rich content with clear citations. Crawls continuously. Most responsive to fixes.
- **ChatGPT**: favors encyclopedic, comprehensive content. Cites Wikipedia 47.9% of the time for factual queries. Prefers well-established sources.
- **Google AI Overviews**: pulls from pages already ranking in top 20 organic results. SEO foundation matters here.
- **Claude**: favors factual accuracy, clear structure, and content that addresses trade-offs honestly.

---

## Step 4 — Optional: Full rewrite mode

If the user explicitly asks for a full rewrite (not just the report), apply all
Section 3-5 fixes to produce a complete AEO-optimized version of the post.

Rules for full rewrite:
- Preserve the author's voice and unique insights — do not genericize
- Keep all original ideas, frameworks, and examples
- Only change **structure and evidence density**, not the substance
- Flag every added element: [AEO: direct answer], [AEO: stat added], [AEO: FAQ]
- Do not invent statistics or sources — use [ADD STAT: topic] as placeholders

---

## Calibration notes

**What this skill does NOT do:**
- Generate llms.txt files (requires full site inventory, not just one post)
- Audit technical crawler access (requires server access)
- Track actual citation performance (requires external monitoring tools)
- Replace keyword research for Google SEO (use substack-seo-metadata-generator for that)

**What makes a post uncitable by design (flag these):**
- Pure personal diary / emotional essay with no searchable question
- Content that requires knowing the author's personal context to make sense
- Posts that are deliberately vague or paywall-teased without a complete free version
- Content in a category where no AI platform cites external sources (e.g., fiction)

If the post falls into one of these categories, say so directly and explain
why AEO optimization won't help, rather than forcing a framework that doesn't fit.

---

## Output language

Always match the language of the input content.
If the Substack post is in Italian, the entire optimization report is in Italian.
If in English, in English.
Do not mix languages in the output.
