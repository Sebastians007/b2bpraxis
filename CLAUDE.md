# B2BPraxis

A B2B company growth system. Guides the full revenue operation from ICP to repeatable pipeline — sessions are persistent, state lives in files.

---

## SESSION START

At the start of every session, read these files if they exist:
1. `GTM.md` — ICP, positioning, sales process, objection map
2. `PIPELINE_TRACKER.md` — current pipeline state, metrics, active deals
3. `PROJECT_STATE.md` — where we left off, decisions made, what's next
4. `ROADMAP.md` — current week's goals and overall 12-week plan

Never ask the user to recap what happened before. The files tell you.

---

## SESSION END

At the end of every session:
1. Update `PIPELINE_TRACKER.md` with any new contacts, replies, stage changes, or closed deals
2. Update `PROJECT_STATE.md`: what was done, what's next, any decisions made and why
3. Update `ROADMAP.md`: mark completed items, note any slippage and why
4. Save any new assets (sequences, proposals, scripts) to `outputs/`

---

## OPERATING RULES

### ICP first — always
Before writing any copy, sequence, or proposal, confirm the ICP is locked. Vague ICP = generic messaging = low reply rates. Push for specificity: industry, company size, revenue, buyer title, user title, trigger event.

### Voice locked before any copy
Before writing a single word of outreach, email sequence, proposal, or LinkedIn message, confirm the brand voice is defined in GTM.md. Define: 3 adjectives that describe the company's voice, 1 thing it would never say, tone for each context (cold outreach, follow-up, proposal, LinkedIn). Every piece of copy must pass this voice before it goes out. No copy without locked voice.

### Messaging hierarchy
Every message must: name a specific pain → cite a specific proof → make a specific ask. Never "we help companies improve their [X]." Always "we helped [company type] [specific result] in [timeframe]."

### Pipeline math is sacred
Always track: outreach volume → open rate → reply rate → meeting rate → close rate → deal size. Know where the leak is before changing anything. Never change two variables at once.

### Fix one thing at a time
If reply rate is low: fix the message (not the channel, not the ICP, not the CTA — just the message). Test, measure, then adjust the next variable. Spray-and-pray optimization breaks the signal.

### Proposals only after discovery
Never send a proposal to someone who hasn't had a discovery call. Proposals sent cold have <5% acceptance rates. A proposal after a good discovery call has >40%.

### Follow up until you know
A non-reply is not a no. Follow up on Day 2, Day 5, Day 10. After Day 10 with no response: archive and revisit in 90 days. The break-up message on Day 10 often converts better than any other touchpoint.

---

## MARKETING TESTING — EXECUTION SQUAD (ES) PROCESS

All outreach campaigns run through this loop. Pipeline math tracks what's happening; ES decides what to do about it.

### The Loop
1. **Define hypothesis** — lock exactly: 1 target audience, 1 painful problem, 1 outcome, 1 price. Nothing vague. This locks into GTM.md before the first message goes out.
2. **Run the experiment** — 10–30 outreach attempts/day. One mode per 7-day sprint (don't mix). Ask each attempt: is the message giving value? Is the angle right?
3. **Make a weekly decision** using hard thresholds (see below) — Scale, Pivot, or Kill. One decision per week. Log it in PIPELINE_TRACKER.md.
4. **Repeat** — data compounds over time. Spin again.

### Decision Thresholds
| Decision | Condition |
|----------|-----------|
| **Scale** | ≥210 attempts + >5% reply rate + 2-3 booked calls |
| **Pivot** | <2% reply rate + 0 booked calls → pivot angle first, not the WHO |
| **Kill** | After pivoting: change subject line, reason for reaching out, CTA type, asset emphasis, tighten "from → to" outcome language |

**Diagnostic rules** (ties directly to pipeline math):
- High attempts, low replies → angle or targeting is weak. Change the message angle first — not the ICP, not the channel.
- Decent replies, low calls booked → CTA or follow-up is weak.
- Calls booked, low close rate → sales process or offer fit issue (not a messaging problem).

### Rules
- One mode per sprint: Mode A (permission ask + customized Loom) or Mode B (evergreen Loom in email). Never mix.
- Pivot angle before pivoting WHO.
- All outreach copy must match the locked voice from GTM.md before it goes out.
- Never change two variables at once — it breaks the signal.
- Log every decision (Scale/Pivot/Kill) in PIPELINE_TRACKER.md with the data that drove it.

---

## CHANGE MANAGEMENT

When refining ICP, messaging, or sequences based on what's working:
1. Document what you're changing and why in PROJECT_STATE.md
2. Keep the original version — never delete, always archive
3. Test the new version on a fresh batch of 25 prospects before declaring it the winner
4. Update GTM.md and outputs/ only after the test confirms the change

---

## SKILL

The `/b2bpraxis` skill handles onboarding new companies and FLOW B audits. After the skill scaffolds this project, session continuity runs from these files. The skill does not need to be re-invoked each session.
