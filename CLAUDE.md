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

Five documents must exist in GTM.md before any prospect is contacted or any content is published. No exceptions — vague targeting and weak offers can't be fixed by better copy.

**PLANNING GATE — print and verify this before any outreach or content begins:**
```
STARTER PACK CHECKLIST
[ ] ICP Mapping Report complete — all 7 dimensions filled (see below)
[ ] Buyer Committee mapped — champion, economic buyer, technical buyer, end user identified
[ ] Competitive Intelligence complete — 3 competitors analyzed, your gap documented
[ ] Audience Deep Research complete
[ ] Offer Memo complete
```
If any item is unchecked, complete it first. Outreach before this checklist is done produces generic messaging that gets ignored.

---

1. **ICP Mapping Report** — lock all 7 dimensions before writing a word of copy:
   - **Firmographic:** industry, company size (employees), revenue range
   - **Technographic:** what tools/stack they use today (signals fit and integration opportunity)
   - **Buyer title:** who signs the check vs who uses the product (often different people)
   - **Trigger event:** what just happened in their world that makes them ready to buy right now (funding round, new hire, regulation change, competitor move, growth inflection)
   - **Buying signals:** what you can see from the outside — hiring patterns for RevOps/SDR/VP Sales roles, job postings naming your category, LinkedIn activity, funding announced in last 6 months
   - **Anti-ICP:** who to explicitly exclude (saves time and protects close rate)
   - **Problem statement:** "When [trigger situation], [buyer title] struggles to [specific pain], which costs them [measurable consequence]."

2. **Buyer Committee Map** — B2B decisions involve multiple people. Map them before outreach:
   - **Champion:** the internal advocate who wants this solved and will push for it
   - **Economic buyer:** who controls the budget and signs off
   - **Technical buyer:** who evaluates fit with existing stack
   - **End user:** who actually uses it day-to-day
   For each: their primary concern, what would make them say yes, what would make them block it. Your champion needs words they can use to sell internally — give them those words.

3. **Competitive Intelligence** — research 3 direct competitors before writing positioning:
   - Feature set and pricing (screenshot their pricing page)
   - Top complaints from real users: check Reddit, G2, Trustpilot, LinkedIn comments — categorize as: pricing too high / missing features / poor UX / bad support
   - What they do well that you must match (table stakes)
   - The specific gap they leave — this is your differentiator, not what you claim, but what their customers are actually asking for
   - Displacement criteria: if a prospect currently uses a competitor, they have budget allocated and a live problem — flag them as high-priority targets

4. **Audience Deep Research** — where they gather (communities, publications, events), what they read, exact language they use to describe their own problems (not your language — theirs), their top 3 objections to buying something like this

5. **Offer Memo** — the specific outcome you deliver, the timeframe, the price, what's included, what's not, the one-line "from → to" statement that a prospect can immediately understand

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

## DISCOVERY CALL

A discovery call is a diagnostic conversation, not a pitch. Show up as a consultant who is figuring out whether to take on the project — not a vendor hoping to win the business. That posture changes the entire dynamic.

### Before the call
- Research the company: industry, size, recent news, obvious problems they're facing
- Know your minimum engagement size before getting on — if the budget is below that, say so early
- Have a notes doc ready — capture their exact words, not your paraphrase of them

### Call structure (30–45 min)

**Opening (2 min):**
"Before I tell you anything about how we work, I want to understand your situation. Mind if I ask a few questions first?" — They always say yes. You've just positioned yourself as the expert in the room.

**Discovery (15–20 min):**
1. "What are you trying to achieve in the next 90 days?"
2. "What have you already tried? What worked, what didn't?"
3. "What does success look like — how would you measure it?"
4. "What's the cost of not solving this?" — the most important question. Makes the value tangible before price ever comes up.
5. "Is there a hard deadline driving this?"
6. "Who else is involved in making this decision?"

**Budget (always ask it):**
"What budget has been set aside for this? I ask so I can tell you honestly whether what you're describing is achievable within that range." — Ask it every time. The salespeople who skip this waste entire proposals on clients who can't afford them.

**Diagnosis (5–10 min):**
Only after you've fully understood their situation — share your read. Not "here's what we'll do" — "here's what we see."
"Based on what you've described, the core issue sounds like [X]. The way we'd approach that is [Y]."
Reference their exact words back to them — it signals you actually listened.

**Next steps (5 min):**
"We'll send a proposal by [specific date]. It'll cover scope, timeline, and investment." Always a specific date. Never "we'll be in touch."

### What not to do
- Don't pitch before you've finished listening
- Don't give away the solution — diagnose, don't prescribe
- Don't leave without a specific next step and a date
- If the fit is clearly wrong, say so: "Honestly, I don't think we're the right fit for this — here's what you actually need." Doing this once builds more trust than 10 polished pitches.

---

## PROPOSALS

A proposal sent cold has <5% acceptance. A proposal after a good discovery call has >40%. The proposal doesn't close the deal — the discovery call does. The proposal makes it official.

### Structure

```
# Proposal: [Project Name]
Prepared for: [Client, Company]
Date: [Date]   |   Valid until: [Date + 14 days]

---

## The Situation
[2-3 sentences restating their problem in their words — shows you listened]

## The Outcome
[What success looks like, using the metrics they gave you on the call]

## Our Approach
[3-5 steps — enough to show thinking, not enough to do it without you]

## What's Included
- [Deliverable 1]
- [Deliverable 2]
- [Timeline]
- [Rounds of revisions / calls included]

## What's Not Included
[Scope boundaries — prevents creep and surprises]

## Investment
$[X,XXX]
Payment: [50% upfront, 50% on delivery — or milestone schedule]

## Testimonial
"[Most relevant quote to this client's situation]" — [Name, Title, Company]

## Next Steps
To move forward: [reply / sign here / send deposit]. We can start [specific date].
```

### Rules
- Send within 24 hours of the call — momentum dies fast
- One page if possible, two max — long proposals get skimmed
- Validity date on every proposal — creates urgency, prevents indefinite ghosting
- Day 3 follow-up if no response: "Wanted to make sure this landed — any questions?"
- Day 7: one line — "Still happy to move forward if the timing works."
- Day 14: soft close — "The start date we were holding is filling up — let us know either way."
- Never discount price without reducing scope. A discount with no scope change signals the original price was inflated.

Save to: `outputs/proposals/[client-name]-[date].md`

---

## PRICING STRATEGY

### Pricing models
- **Project-based:** fixed price for a defined scope. Use when the deliverable is clear and bounded.
- **Retainer:** monthly fee for ongoing access or output. Price on the outcome, not hours. Include a 3-month minimum — month-to-month retainers cancel at the first budget squeeze.
- **Value-based:** price as a percentage of value created. Use for high-leverage work where the client's upside is measurable and large.
- **Hourly:** never. It punishes efficiency and caps revenue. If a client insists, translate to a project rate.

### Positioning the price
Never lead with price. Lead with the outcome and let the price follow from it:
- Not: "We charge $X for this"
- Yes: "Our typical engagement for this type of work runs $X–Y depending on scope. Our last client in your situation saw [specific metric] within [timeframe]."

### Three-option anchoring
Always present three scope options (smaller, right-sized, premium). Most buyers choose the middle. This isn't manipulation — it helps buyers make decisions and ensures clients who want more can access it.

### Negotiation
- "That's too expensive" → "Compared to what?" Find out if it's the total or the timing. Then: "If this produces [specific result], is the investment still too high?"
- If genuinely too expensive for their budget: "We could start with [smaller scope] at $Y. That's usually enough for both sides to know if we should continue."
- Never drop the rate — drop the scope. "I can do [reduced version] for that budget. Here's exactly what that covers."

### Annual retainers
Offer annual retainers at a 15–20% discount. Annual = guaranteed cash flow on your side; the discount is worth it. Clients on annual retainers almost never churn mid-engagement.

---

## OBJECTION HANDLING

The four objections that stall B2B pipelines — and how to address each without flinching.

### "That's too expensive"
Find out which of three things it actually means before responding: (1) they didn't understand the value, (2) they're comparing to the wrong benchmark, or (3) they genuinely can't afford it.

**Unpack it:** "Is it the total number, or is it the timing?" — Often it's one, not both. Learn which first.

**Reframe to ROI:** "Help me think about this with you — what would [the outcome] be worth to the business over the next 12 months?"

**Smaller entry:** "If the full engagement feels like a big commitment before we've worked together, we sometimes start with [smaller scope] at $Y. That usually answers the fit question for both sides."

Never drop the rate without dropping scope. It tells the client your original price wasn't real.

### "Not right now"
Find out if it's real or a brush-off before accepting it.

**Ask what changes it:** "What would need to be different for this to make sense?" — A real answer means it's timing. No answer means it's a soft no.

**Get a date:** "Understood — when should I follow up? Next quarter? After [specific trigger]?" No date = never.

**90-day nurture:** timing objections go into a 90-day follow-up sequence, not the dead pile. Circumstances change. The company that couldn't budget in Q1 often can in Q3.

### "We're evaluating other vendors"
Good — they're serious about solving the problem. Your job is to be the easiest choice.

**Get on the scorecard:** "What criteria are you using to decide?" — Get them to name it. Then address each criterion specifically in your follow-up.

**Differentiate on process:** what you do is similar to competitors. How you work — communication, accountability, rigor — is usually the real differentiator. Make it visible.

**Follow up with value:** while they're evaluating, send one relevant resource (case study, insight). Shows you're thinking about their problem. Doesn't feel like chasing.

### "I need to get internal buy-in"
The real decision-maker isn't in the room. Your job is to get in the room.

**Ask to join the conversation:** "Would it be useful if I joined a call to answer questions directly? I can put together a one-pager tailored to their concerns if that would help."

**Give them the words:** send a summary they can forward internally. Include: the problem, the approach, the expected outcome, the investment, one relevant case study. A champion who has a proposal in hand closes buy-in at 3x the rate of one who's explaining a conversation.

---

## CLIENT ONBOARDING (POST-CLOSE)

Most of the client relationship is won or lost in the first two weeks. The gap between signed contract and first deliverable is where client anxiety peaks. Fill it deliberately.

### Within 48 hours of signing
Send a kickoff email immediately — not after you've planned everything, immediately. It confirms they made the right decision.

Structure:
- "Excited to get started — here's what happens next"
- Your first 3 steps with dates
- What you need from them (access, documents, contacts) — listed specifically, not vaguely
- The kickoff call invite (scheduled in the same email)

### Kickoff call agenda
1. Reconfirm the goal in their words — let them say it, not you
2. Lock success metrics — specific and measurable. No metrics defined = no way to prove value later.
3. Communication agreement: one channel, check-in cadence, who approves what
4. First deliverable: specific day, specific output
5. "Is there anything you're worried about or want to flag?" — ask it. Concerns surfaced early are fixable; concerns surfaced late damage trust.

### First deliverable
Ship something within 5 business days. It can be an outline, draft, or research summary — not the final output. Early momentum is the most powerful signal that the client made the right choice.

Never disappear for two weeks. Silence in the first two weeks = buyer's remorse.

### Capture everything promised
In GTM.md, document what was promised in the proposal and discovery call. If any expectations were set verbally that aren't in the proposal, capture them in a kickoff summary sent within 24 hours of the kickoff call. This is your scope protection document.

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

## CONTENT STRATEGY

The ES loop fills the pipeline now. Content fills it over time at lower cost. Run both — outbound is the accelerator, content is the compounding asset.

### 3-pillar structure
Every piece of content fits one pillar. Weekly mix: 2 Authority/Process : 1 Proof.

| Pillar | Purpose | Examples |
|--------|---------|---------|
| **Authority** | Demonstrates expertise — what you know | Frameworks, breakdowns, contrarian takes, "why X doesn't work" |
| **Proof** | Shows results — what you've done | Case studies, before/after stats, client outcomes, recent wins |
| **Process** | Shows how you work | Behind-the-scenes, methodology breakdowns, project updates |

### Cadence
- 3 posts per week on LinkedIn minimum
- Gateway post (resource offer) once per week max — more than that and the feed becomes transactional
- Batch-write on Mondays: draft the week's posts in one session, schedule them out. One writing session per week beats daily scramble every time.

### Post structure
- Hook (first line): specific result, provocative claim, or pattern interrupt. The hook decides whether the scroll stops.
- No "I" as the first word — reads as self-promotional before they've read anything
- 3–5 punchy lines or a brief structured breakdown — no walls of text
- End with a question or insight, not a CTA — algorithm favors conversation, not pitches
- Gateway posts are the exception: these end with "Comment [WORD] to get it"

### What to write about
Read `GTM.md` Audience Deep Research before planning content. Write about:
- Problems your ICP describes in their own language — not your language
- Decisions your ICP makes regularly — help them make better ones
- Mistakes you see most often in your category
- Your own process and approach — this is the most differentiated content you can produce

### Content calendar
Keep a simple `content/CALENDAR.md`:
```
| Date | Pillar | Topic | Hook (first line) | Status |
|------|--------|-------|-------------------|--------|
| [date] | Authority | [topic] | [first line] | Draft |
```
Plan 2 weeks ahead. Never post without a hook written first — the hook is what decides whether the post gets read.

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
