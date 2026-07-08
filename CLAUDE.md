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

## STARTER PACK (required before any outreach or content)

Three documents must exist in GTM.md before any prospect is contacted or any content is published. No exceptions — vague targeting and weak offers can't be fixed by better copy.

1. **ICP Mapping Report** — industry, company size, revenue range, buyer title, user title, trigger event (what just happened in their world that makes them ready to buy), buying signals (what you can see from the outside that indicates a good fit)
2. **Audience Deep Research** — where they gather (communities, publications, events), what they read, exact language they use to describe their own problems (not your language — theirs), their top 3 objections to buying something like this
3. **Offer Memo** — the specific outcome you deliver, the timeframe, the price, what's included, what's not, the one-line "from → to" statement that a prospect can immediately understand

---

## INBOUND & NURTURE

Outbound (ES loop) fills the pipeline now. Inbound fills it at lower cost over time. Run both. The 3-layer trust system builds inbound authority while outbound runs.

### Layer 1 — Generate

**Gateway posts:** Publish a value-first LinkedIn post offering a free resource (guide, template, case study). Prospect comments → resource auto-delivered via DM → email captured → enters nurture. Post structure: hook (the result the resource produces) → what's inside → "Comment [WORD] to get it."

**Outbound:** ES loop handles this. Layer 1 outbound = 30 connection requests + 10 cold emails per day max. Value-first framing only — never open with a pitch. Send a guide, a relevant insight, or a case study. No pitch in the first touch.

**Build order:** outbound first → email nurture content second → LinkedIn posting third → retargeting ads last. Never start with ads. Ads amplify what's already working — they don't create it.

### Layer 2 — Nurture

**Lead scoring:**
| Stage | Signals | Action |
|-------|---------|--------|
| Cold | Downloaded a resource, connected on LinkedIn, no further engagement | Enter 90-day email sequence |
| Warm | Opened 3+ emails, clicked 2+ links, revisited the site | Increase touch frequency, send higher-value asset |
| Hot | Visited pricing or case study pages repeatedly, replied to email, engaged with multiple assets | Flag for direct outreach — move to Layer 3 |

**Email nurture sequence rules:**
- 90+ days minimum. Most B2B buyers take 3-6 months to be ready.
- Every email links to a resource (guide, video, case study) — never directly to a sales page
- Rotate content type: insight → case study → white paper → video snippet → tool/template. Never the same format twice in a row.
- Tone matches the locked voice in GTM.md throughout — the sequence should feel like the same person talking, not a drip campaign

**Never-discard rule:** A lead who doesn't convert now is not a dead lead. Archive them at 90 days with no engagement, revisit at 6 months. Circumstances change. The ones who come back pre-sold close faster and cheaper than cold leads.

**Retargeting:** run presence-building ads to your warm list — case studies, client outcomes, short video clips. Not sales pitches. Rotate assets every 2 weeks. The goal is to stay visible, not to convert directly from an ad.

### Layer 3 — Convert

Hot leads auto-flagged in PIPELINE_TRACKER.md → direct outreach with a specific, relevant angle (reference what they engaged with) → assessment page → value bridge → book call → pre-call nurture → discovery call. See PRE-CALL CONVERSION section.

---

## PRE-CALL CONVERSION

The gap between "interested" and "showed up to the call" is where most pipeline leaks. These three steps close it.

### Assessment Page
Before booking a call, hot prospects complete a short assessment (2-3 minutes). Structure: simple qualifying questions first → specific pain questions last (most painful question second-to-last, not last — end on a forward-looking note). The arc builds from easy to uncomfortable to hopeful. Two purposes: (1) qualifies the lead so both sides know if it's worth a call, (2) primes the prospect by surfacing their own pain before they talk to you. Never send a booking link cold — the assessment filters and prepares.

### Value Bridge
Immediately after booking: send a short explainer (3-minute video or 1-page PDF) that explains your process, not your credentials. "Here's exactly how we approach [their problem]." If they don't understand the process, they don't show up. The value bridge turns a calendar hold into a committed meeting.

### Pre-Call Nurture Sequence
- **Never book calls more than 7 days out** — the further out the call, the lower the show rate
- Send confirmation + value bridge within 1 hour of booking
- Day 3 before call: relevant case study or short insight — something specific to their industry
- Day of call (morning): "Looking forward to speaking at [time]. We'll cover [specific thing]." One sentence. No fluff.
- Target: 80%+ show rate. If below 70%, the value bridge or booking process needs work — diagnose before blaming no-shows

---

## CLIENT SUCCESS & REFERRALS

### Client Success
Getting the client is step one. Keeping them and expanding is where the margin lives.

- **Week 1:** proactive check-in — not "how's it going" but "here's what I noticed in the first week and here's what we're doing about it." Sets the tone that you're ahead of problems, not behind them.
- **Monthly:** send a short progress summary tied to the metrics defined at project start. No metrics defined at start = no way to demonstrate value. Always lock success metrics before work begins.
- **Expansion signals:** client mentions a problem adjacent to your scope → flag it immediately. "That's actually something we also help with — want me to put together a quick scope?" Expansion revenue closes at 3x the rate of new business.
- **30-day post-project check-in:** after delivery, follow up to see how results are performing. Most freelancers disappear at invoice. This one email generates more referrals than any other touchpoint.

### Referral System
Referrals are the highest-converting lead source in B2B. They close faster, negotiate less, and trust more. Most companies get them by accident. This makes it systematic.

**Ask timing:** within 48 hours of a client saying something positive — mid-project when momentum is high, not at project end when they're thinking about invoices. Strike when the emotion is fresh.

**The ask:**
```
"Glad this is going well. Most of our best clients come through referrals.
Is there anyone in your network dealing with [exact problem you solve]?
Here's a line you could forward if someone comes to mind:

'[Company] helped us [specific result]. Happy to intro if it's relevant.'"
```

Always give them the words. Forwarding a pre-written line takes 10 seconds. Writing their own referral from scratch takes effort they won't spend.

**Partner network:** identify 5-10 companies that serve your ICP but don't compete. Build actual relationships — refer to them first, unprompted. Reciprocity is real. Once the relationship is warm, make it explicit: "I think there's a good referral flow here — want to be intentional about sending each other leads?"

**Track in PIPELINE_TRACKER.md:**
```
| Referral Source | Type | Last Referral | Total Referred |
|----------------|------|---------------|----------------|
```

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
