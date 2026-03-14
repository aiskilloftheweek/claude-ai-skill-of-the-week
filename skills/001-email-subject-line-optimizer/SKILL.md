---
name: email-subject-line-optimizer
description: Analyzes a subject line against proven best practices and generates 5 optimized alternative versions. Use this skill whenever the user wants to improve, test, or rewrite an email subject line. Trigger on phrases like "improve this subject line", "optimize the subject", "write a better subject line", "suggest subject line alternatives", "this subject line isn't converting", "help me with the subject line", "rewrites for the subject", or when the user pastes an email and asks specifically about the subject line (not the full body). Also trigger when the user uploads or pastes an email and says "can you improve the subject?" or similar. Do NOT trigger this skill for full email body rewrites — use email-copywriter-optimizer for that.
---
 
# Email Subject Line Optimizer
 
You receive an email subject line (and optionally the email body for context) as input.
 
Your job: analyze the subject line against the best practices below, diagnose its weaknesses, and produce **5 optimized alternative versions** — each using a different psychological angle.
 
---
 
## Process
 
### Step 1 — Silent analysis
 
Before writing anything, internally evaluate the subject line across these dimensions:
 
**Length & mobile readability**
- Is it under 50 characters? (ideal: 30–50 chars; under 30 for mobile-first)
- Will it get truncated on mobile screens?
- Does it front-load the most important word/concept?
 
**Clarity vs. cleverness**
- Is it specific or vague/generic?
- Does it make a clear promise or does it try to be cryptic?
- Would the reader know what the email is about after reading it?
 
**Psychological trigger**
- Which primary trigger does it use (or fail to use)? FOMO, curiosity, pain point, benefit, personalization, social proof, urgency, humor?
- Is the trigger genuine or does it feel forced/spammy?
 
**Spam risk**
- Does it use all caps, excessive punctuation, or known spam trigger words?
- Does it make unverifiable claims ("FREE MONEY", "GUARANTEED")?
 
**Deliverability signals**
- Does it contain words commonly flagged by spam filters?
- Is it formatted cleanly (no weird symbols, no misleading previews)?
 
**Alignment with email content**
- If the body was provided: does the subject line accurately reflect the email's main value?
- Is there a mismatch between promise (subject) and delivery (body)?
 
---
 
### Step 2 — Output
 
Produce this structured output:
 
---
 
## 🔍 Subject Line Audit
 
**Original subject:** `[the subject line as provided]`
 
A concise diagnosis (3–5 lines) identifying:
- What works (if anything)
- The 2–3 main weaknesses reducing open rates
- The primary psychological lever that's missing or underused
 
---
 
## ✏️ 5 Optimized Alternatives
 
For each alternative, provide:
- The subject line (formatted as inline code)
- The character count
- The psychological angle it uses
- One sentence explaining why it works
 
Format:
 
---
 
**1. [Label: e.g., Curiosity Gap]**
`[Subject line here]` — *[X chars]*
**Angle:** [Psychological trigger]
**Why it works:** [One sentence explanation]
 
---
 
Repeat for all 5 alternatives.
 
---
 
## 💡 Recommendation
 
One short paragraph (3–4 lines) indicating:
- Which of the 5 alternatives is the strongest pick and why
- What to A/B test (e.g., version 1 vs. version 3)
- One optional tip on the preview text to pair with the winning subject
 
---
 
## Reference: Subject Line Best Practices
 
### Length
- Optimal: **30–50 characters** for desktop; **under 30** for mobile-first audiences
- Over 60 characters: truncated on most mobile clients — the key message disappears
- Short ≠ vague. Short + specific is the winning formula
- Front-load: the most compelling word or phrase goes first, not at the end
 
### Psychological triggers (use one primary angle per subject line)
 
| Trigger | How to use it | Example |
|---|---|---|
| **FOMO / Urgency** | Real deadlines, limited availability | "Last 6 hours: your spot expires tonight" |
| **Curiosity gap** | Open a loop the reader must close by opening | "The mistake 90% of founders make on day one" |
| **Pain point** | Name a specific problem your audience has | "Still losing leads after the first call?" |
| **Benefit / value** | State a clear, concrete outcome | "3 templates that saved me 4h/week" |
| **Personalization** | Name, role, company, behavior, location | "Luca, your October report is ready" |
| **Social proof** | Numbers, peers, recognition | "How 1,200 solopreneurs grew their list this month" |
| **Humor** | Unexpected twist, self-aware joke | "We'd be better together (said the email to the inbox)" |
| **Straightforward** | No tricks — just clarity. Works when trust is established | "Your invoice for October" |
 
### Words & formatting that work
- **Numbers**: signal concrete, scannable value — "5 subject line fixes", "doubled open rates in 3 weeks"
- **[Brackets]** and **{Curly braces}**: create visual contrast in the inbox — "[NEW]", "{Quick question}"
- **Verbs that imply action or change**: discover, stop, avoid, steal, fix, unlock
- **Questions**: engage the reader's brain before they open — but avoid yes/no questions with obvious answers
- **"You" in triggered/transactional emails**: works well (it's personal); avoid in broadcast campaigns (feels like a sales pitch)
 
### Words & formatting to avoid
- ALL CAPS (except strategic 1-word emphasis like "FREE" — use sparingly)
- Multiple exclamation points!!!
- Classic spam trigger words: "guaranteed", "act now", "earn money", "click here", "no risk", "100% free"
- Vague openers: "Newsletter #14", "Check this out", "Important update", "Quick question" (overused in cold email)
- Misleading hooks that the email doesn't deliver on — kills trust and future open rates
 
### Personalization
- Including the recipient's first name boosts open rates by ~10–14% across industries
- Beyond the name: city, company, recently viewed product, membership tier, behavior-based triggers
- Always set a fallback for missing data — "Hi [FNAME]" errors destroy credibility
 
### Emoji usage
- A single relevant emoji increases open rates by ~45% (Experian data) in B2C contexts
- Use max 1–2 emojis per subject line
- Place at the start or end — not embedded mid-sentence
- Don't replace words with emojis (e.g., "I ❤️ this" is fine; "I ❤️ ur 🛒" is not)
- Test rendering: emojis display differently across Gmail, Outlook, Apple Mail
- Avoid in formal B2B, legal, financial, or sensitive contexts
 
### A/B testing guidance
- Test **one variable at a time**: length, tone, trigger type, personalization, emoji presence
- Need minimum ~1,000 recipients per variant for statistically significant results
- Let the test run at least 4 hours before declaring a winner
- Build a testing log: what you tested, which won, why — it compounds over time
- High-value tests: question vs. statement, short vs. medium, benefit vs. curiosity, emoji vs. no emoji
 
### The preview text pairing rule
The subject line and preview text function as a two-part pitch. Never write one without considering the other.
- Preview text: max 50 characters, front-loaded with the key message
- It must **complement** the subject, not repeat it
- Think of it as: subject = hook, preview = the reason to open
- If left empty, email clients auto-pull the first line of body copy (often "View in browser" — a wasted opportunity)
 
### Deliverability & spam filters
- Subject lines are the primary spam filter trigger — 69% of recipients mark email as spam based on the subject alone (Zippia)
- Avoid deceptive RE: or FWD: prefixes on cold/broadcast email
- Don't use "$$$", "FREE FREE FREE", or excessive symbols
- Consistent sender name + relevant subject = improved sender reputation over time
 
---
 
## Quick reference: 5 angles to always consider
 
When generating alternatives, cover at minimum these 5 psychological angles:
 
1. **Curiosity/open loop** — what question does the reader need to answer?
2. **Pain point** — what problem are they actively trying to solve?
3. **Concrete benefit** — what specific, measurable outcome do they get?
4. **Urgency/scarcity** — is there a real reason to open now vs. later?
5. **Social proof or authority** — who else is doing this / what do the numbers say?
 
