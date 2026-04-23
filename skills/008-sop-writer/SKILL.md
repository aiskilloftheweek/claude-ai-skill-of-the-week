---
name: sop-writer
description: >
  Transforms any process description — however rough, incomplete, or disorganized — into
  a clear, delegatable Standard Operating Procedure (SOP). Use this skill every time the
  user wants to document a process, create a procedure for a team member or VA, build
  an operations manual, standardize a workflow, or says things like "write an SOP for this",
  "help me document this process", "I need to delegate this", "create a procedure for my VA",
  "turn this into a checklist someone else can follow", "document how I do X", or pastes
  any description of how they do something and wants it structured. Always trigger this
  skill when the goal is to make a process repeatable and delegatable — even if the user
  phrases it casually or informally.
---
 
# SOP Writer
 
Turns any process description — bullet points, voice transcripts, half-explained workflows,
or detailed outlines — into a structured, delegatable Standard Operating Procedure.
 
The output is always specific, tool-aware, edge-case-aware, and ends with a built-in
delegability test. It works for solopreneurs, ops managers, and founders alike.
 
---
 
## Before you start
 
Read the user's input carefully and classify it into one of these input types:
 
| Type | Signals | Action |
|---|---|---|
| **Verbal / stream of consciousness** | Informal, jumps around, missing sequence | Run full elicitation (3.2) |
| **Disorganized bullets** | Has structure but missing tool/trigger/output details | Run partial elicitation (3.3) |
| **Semi-structured description** | Steps in order, some tools mentioned | Fill gaps only, then produce |
| **Loom transcript / audio dump** | Long, repetitive, with digressions | Extract, then confirm before producing |
 
If the input is too vague to even classify, ask one question only:
*"Can you describe what happens from start to finish when you run this process — even roughly?"*
 
---
 
## Step 1 — Identify the SOP type
 
Before eliciting or producing anything, classify the process into one of these types.
The type determines the output format (see Section 4).
 
- **Type A — Delegation to VA/contractor**: process will be executed by someone external
- **Type B — Editorial / content process**: publishing, writing, content workflows
- **Type C — Onboarding**: new client, new hire, new tool rollout
- **Type D — Recurring operational**: daily/weekly/monthly repeating tasks
- **Type E — Crisis / exception handling**: non-standard situations, escalations
If unclear from input, infer from context. If still unclear, ask:
*"Who will be running this process — you, or someone else?"* and
*"Is this something that happens on a schedule, or when something specific occurs?"*
 
---
 
## Step 2 — Elicitation logic
 
### The 6 mandatory fields
 
Before writing the SOP, you need these. Extract them from input if present.
If missing, ask for them using the decision logic below.
 
1. **Process name** — what is this SOP called?
2. **Executor** — who runs it? (role, not person name)
3. **Trigger** — what causes this process to start?
4. **Expected output** — what is objectively true when the process is done correctly?
5. **Tools involved** — which apps, platforms, or software are used? (include obvious ones like email, Google Drive)
6. **Frequency** — how often does this run?
### Decision logic: when to ask vs. when to infer
 
```
Count missing mandatory fields:
 
3 or more missing → Ask in one block, max 3 questions at a time
1–2 missing       → Ask 1 question, then proceed
0 missing         → Produce the SOP directly
```
 
Never ask more than 3 questions per turn. Never run a questionnaire.
Behave like an ops consultant extracting information in conversation, not a form.
 
### Elicitation question bank (use as needed, never all at once)
 
**For trigger and output (highest priority):**
- "What kicks this process off — does something arrive, does a day of the week come, does someone ask you something?"
- "When this process is finished correctly, what's different in the world? What can you point to and say 'done'?"
**For tools and executor:**
- "Which tools or platforms get touched during this process? Even basic ones like email or Docs."
- "Who will actually run this — you, a VA, a team member?"
**For edge cases (this is the differentiator — always ask if not mentioned):**
- "Has this process ever gone wrong? What happened?"
- "Is there any step where the person running it has to make a judgment call or 'figure something out'?"
**For frequency and variants:**
- "How often does this run?"
- "Is there a 'normal' version and an 'urgent' or 'exception' version?"
### Graceful degradation rule
 
If the user doesn't provide all fields, never invent steps or details.
- **Infer** what you can from context (e.g., "you mention Notion → tool is Notion")
- **Mark** unresolvable gaps with `[TO COMPLETE]`
- **Never fabricate** specific steps, tool names, or criteria not described by the user
---
 
## Step 3 — Determine output format
 
Ask (or infer from context) where this SOP will live:
 
| Destination | Output format |
|---|---|
| Notion / Obsidian | Markdown with section emoji |
| Google Docs / Word | Clean Markdown, no emoji |
| ClickUp / Asana | Flat numbered steps, no nesting |
| Email to VA | Flowing text, steps in bold |
| Not specified | Default: Markdown with emoji |
 
Also determine **detail level** based on executor:
- **Executor = VA or external collaborator** → Expanded format (include where to click, what to type)
- **Executor = founder / user themselves** → Compact format (one line per step)
---
 
## Step 4 — Write the SOP
 
Use the **Universal Base Structure** below, then apply the **Type Variant** on top.
 
### Universal Base Structure
 
```markdown
# [PROCESS NAME]
 
**Version:** 1.0 | **Created:** [date] | **Review by:** [date + 6 months]
 
---
 
## 📋 Process overview
- **Executed by:** [role]
- **Trigger:** [what starts this process]
- **Frequency:** [how often]
- **Estimated time:** [X minutes / hours]
- **Expected output:** [what is objectively true when done]
 
---
 
## 🛠️ Tools required
- [Tool name] — [what it's used for]
- [Tool name] — [what it's used for]
 
---
 
## 📝 Steps
 
1. **[Action verb] [what]** — [where / in which tool]
2. **[Action verb] [what]** — [where / in which tool]
3. ...
 
---
 
## ⚠️ Edge cases & exceptions
 
- If [situation X occurs] → [do Y instead]
- If [something is missing] → [escalate to / default to]
- If unsure → [decision rule or who to contact]
 
---
 
## ✅ Completion checklist
 
- [ ] [Verifiable output 1]
- [ ] [Verifiable output 2]
- [ ] [Verifiable output 3]
 
---
 
## ❓ FAQs
 
**Q:** [Question someone running this for the first time would ask]
**A:** [Answer]
 
---
 
## 🧪 Delegability test
 
Before handing this SOP to someone else, verify:
 
- [ ] Someone with zero context on this process could complete it using only this document
- [ ] Every tool mentioned is accessible to whoever will run this
- [ ] The edge cases section covers situations that have actually occurred
- [ ] The expected output is verifiable — not subjective
 
→ If any answer is NO, note which section needs revision before delegating.
```
 
---
 
### Type variants (apply on top of base structure)
 
**Type A — Delegation to VA/contractor**
- Expand the FAQs section to 5–7 questions
- Add under each complex step: *"If unclear, [specific action]"*
- Add at the end: **"Escalation path"** — who to contact, how (Slack/email), response time expected
- Use expanded step format: break every step into sub-steps (3a, 3b, 3c)
**Type B — Editorial / content process**
- Add after Steps: **"Quality criteria"** — specific, objective standards
  (e.g., "Title must be under 60 characters", "Cover image must be 1600×840px")
- Add: **"Common mistakes"** — 3–5 things that go wrong and how to spot them
**Type C — Onboarding**
- Replace "Frequency" with "Timeline"
- Structure steps by time: **Day 1 / Week 1 / Month 1**
- Add: **"Milestones"** — checkpoint events that confirm onboarding is on track
- Add: **"Success criteria at 30 days"**
**Type D — Recurring operational**
- Add estimated time per step alongside each step
- Add: **"Anomaly signals"** — early warning signs that something is going wrong
- Compress FAQs; expand Completion checklist instead
**Type E — Crisis / exception handling**
- Lead with a **decision matrix** before the steps:
  ```
  IF [condition A] → Go to Step 3
  IF [condition B] → Go to Step 7
  IF [condition C] → Escalate immediately (see Step 11)
  ```
- Label every step with severity: `[CRITICAL]` / `[STANDARD]` / `[OPTIONAL]`
- Add: **"Post-resolution checklist"** — what to document and communicate after the crisis
---
 
## Step 5 — Final output check
 
Before delivering, verify:
 
- [ ] Every step uses an active verb ("Open", "Click", "Send", "Copy" — not "You should" or "It is recommended")
- [ ] Every tool mentioned by name is one the user confirmed exists in their process
- [ ] At least one edge case is included — even for simple processes
- [ ] The Delegability Test block is present at the end
- [ ] No steps were invented that weren't described or clearly inferable from the user's input
- [ ] Format matches the destination (Markdown / flat text / etc.)
- [ ] Detail level matches the executor (expanded for external / compact for self)
---
 
## Example: compact input → full output
 
**User input:**
*"When I get a new client inquiry from the contact form, I check if they fit, schedule a call, and send them the onboarding doc after."*
 
**What the skill does:**
1. Classifies: Type C (onboarding), executor unclear → asks "Who runs this — you or a team member?"
2. Identifies missing fields: tools, trigger specifics, expected output, edge cases
3. Asks (max 3): "Which tools do you use for scheduling and sending the onboarding doc?" + "What makes someone a 'fit' — is there a criteria list?"
4. Produces SOP with decision criteria for fit/no-fit as an edge case, specific tool steps, and delegability test
---
 
## Notes
 
- Always produce the SOP in the same language the user is writing in, unless they specify otherwise
- If the process is very simple (under 5 steps, no tools, no edge cases), still produce the full structure — the value is in the format, not just the steps
- If the user says "just give me the steps, no template", respect that and produce a clean numbered list — but always append the Delegability Test at the end, as a minimum
 
