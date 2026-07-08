# Skill: b2bpraxis

A B2B company growth system for Claude. Guides a company from ICP definition to repeatable revenue — or picks up an existing sales operation and gets it back on track. Sessions are persistent, state lives in files.

**Install:** Copy this file to `~/.claude/skills/b2bpraxis.md`
**Invoke:** `/b2bpraxis` in any company folder

---

## On invoke — detect which flow to run

Check the current folder for:
- `GTM.md` or `PIPELINE_TRACKER.md` → existing operation, run FLOW B
- `outputs/sequences/` or `outputs/proposals/` with files → existing assets, run FLOW B
- Neither → new start, run FLOW A

Tell the user which flow you're running and why in one line.

---

## FLOW A — New B2B Operation

### Step 1: Clarity interview — ask all 8 in one message

```
1. What does your company sell, and what's the #1 outcome you deliver for clients?
   (e.g. "We cut SaaS churn by 30% using behavioral email automation")

2. Describe your ideal customer profile (ICP) as specifically as possible:
   Industry / company size / revenue range / title of buyer / title of user

3. What's your average deal size and typical sales cycle length?

4. How are you currently generating leads? (inbound, outbound, referrals, partnerships — be specific)

5. What channels do you want to use for outreach?
   Cold email / LinkedIn / Cold calling / Events / Content / Partnerships

6. What does your current sales process look like?
   (Even if informal — how does a prospect go from first contact to signed contract?)

7. What's your revenue target for the next 90 days?

8. What is explicitly NOT in scope for now?
   (scope lock — prevents spreading effort too thin)
```

Wait for all 8 answers before proceeding.

### Step 2: ICP stress test

Before building anything, pressure-test the ICP and value proposition:

- **Pain test:** Does the problem you solve cause companies to actively spend money trying to fix it right now?
- **Specificity test:** If you showed your ICP definition to 10 sales reps, would they all target the same kind of company?
- **Proof test:** Do you have at least 2 clients who match this ICP and got the result you're promising?
- **Reach test:** Are there enough companies matching this ICP to hit your 90-day revenue target?
- **"Why you" test:** Why would this ICP choose you over an alternative? Name the real differentiator.

Give a verdict: ✅ STRONG / ⚠️ REFINE / 🔄 REFRAME. Fix before continuing.

### Step 3: Scaffold the operation

Generate these files:

**GTM.md** — go-to-market spec covering:
- ICP definition (industry, size, revenue, buyer title, user title, trigger events)
- Value proposition: one sentence, one paragraph, elevator pitch
- Competitive positioning: how you're different from the 3 most likely alternatives
- Pricing tiers and deal structure
- Sales process stages with entry/exit criteria per stage
- Objection map: top 5 objections + how to handle each
- Success metrics: leading indicators (outreach volume, reply rate, meetings) and lagging (pipeline, revenue)

**PIPELINE_TRACKER.md** — copy from templates/PIPELINE_TRACKER.md, populate with ICP and goals

**PROJECT_STATE.md** — starting state:
- Date started
- ICP confirmed
- Channels selected
- 90-day revenue target
- What's done: nothing yet
- What's next: messaging framework → outreach sequences → first send

**ROADMAP.md** — generate the 12-week aggressive roadmap (see Roadmap section below)

**CLAUDE.md** — scaffold with these session rules:
```
At START of every session:
  Read GTM.md — understand ICP, positioning, and sales process
  Read PIPELINE_TRACKER.md — know current pipeline state
  Read PROJECT_STATE.md — know exactly where we left off
  Read ROADMAP.md — know what's due this week

At END of every session:
  Update PIPELINE_TRACKER.md with any new contacts, replies, or stage changes
  Update PROJECT_STATE.md: what was done, what's next, decisions made
  Update ROADMAP.md: mark completed items, flag slippage
  Save any new outputs (sequences, templates, proposals) to outputs/
```

### Step 4: Build the messaging framework

Before writing any sequence, build the messaging foundation:

**Messaging brief** (save to `outputs/messaging.md`):
- Hook variants (3): different angles for the same value proposition
- Problem framing (3 versions): how to describe their pain without sounding generic
- Proof point: the specific result, for a specific client type, in a specific timeframe
- CTA options: meeting / reply / resource — which to use and when

### Step 5: Build outreach sequences per channel

For each channel selected in the interview, generate a full sequence:

**Cold email sequence** (`outputs/sequences/cold-email.md`):
- Email 1 (Day 1): Pattern interrupt + specific pain + one-line proof + low-friction CTA
- Email 2 (Day 3): Different angle, shorter, reference email 1
- Email 3 (Day 7): Value add (insight, resource, relevant stat) + CTA
- Email 4 (Day 14): Break-up email — "last one, no hard feelings"
- Subject line variants (A/B test): 3 options per email

**LinkedIn sequence** (`outputs/sequences/linkedin.md`):
- Connection request note (300 chars max): no pitch, just relevance
- Follow-up DM 1 (Day 2 after connect): trigger-based opener + value
- Follow-up DM 2 (Day 5): social proof + CTA
- Follow-up DM 3 (Day 10): short, direct, last attempt

**Cold call script** (`outputs/sequences/cold-call.md`) if selected:
- Opening (5 sec): name + company + permission
- Bridge (15 sec): why this person, why now — specific trigger
- Value statement (10 sec): result for similar company
- Qualifying question (to get them talking)
- Objection handlers for top 3 objections
- CTA: meeting, email follow-up, or next step

### Step 6: Confirmation gate

Present GTM.md, messaging framework, and sequences. Wait for confirmation before any outreach goes out.

---

## FLOW B — Existing B2B Operation

### Step 1: Audit the current state

Ask the user to share:
- Any existing sequences or outreach templates (paste or describe)
- Current pipeline: how many prospects at each stage right now
- What's been sent: volume, open rates, reply rates if known
- Last 3 clients won: how they came in, how long the cycle was
- Biggest blocker right now: outreach volume, reply rate, close rate, or average deal size

### Step 2: Diagnose the revenue gap

Map the funnel and find where it breaks:

```
## Revenue Funnel Audit

Outreach volume: [#/week] → Is this enough to hit target? (Rule: 100 touches/week minimum for $10K MRR target)
Open rate: [X]% → Benchmark: >40% (if below, subject line problem)
Reply rate: [X]% → Benchmark: >5% cold (if below, message problem or wrong ICP)
Meeting rate: [X]% of replies → Benchmark: >40% (if below, CTA or qualification problem)
Close rate: [X]% of meetings → Benchmark: >25% (if below, demo/proposal problem or wrong ICP)
Average deal: $[X] → Does this math reach the 90-day target?

Diagnosis: [Single sentence — where is the biggest leverage point right now?]
```

Present this diagnosis. Fix the biggest gap first.

### Step 3: Assess existing assets

Audit every existing asset:
- Sequences: are they specific to the ICP or generic? Is the proof real or vague?
- ICP definition: is it precise enough that two reps would target the same company?
- Proposals: do they lead with the client's outcome or with your services?
- Objection handling: is it documented or in people's heads?

Flag what needs to be rewritten vs. what's working.

### Step 4: Scaffold missing files

Create any of these that don't exist:
- GTM.md (from audit findings)
- PIPELINE_TRACKER.md
- PROJECT_STATE.md (from current state)
- CLAUDE.md (with session continuity rules)
- ROADMAP.md (from current position — see Roadmap section)

Show the current week they're at, mark earlier weeks done, show remaining roadmap from here.

---

## Roadmap — 12-Week Aggressive B2B Revenue Build

Generate tailored to their specific situation. In FLOW B, identify which week they're equivalent to and start there.

```
## Where You Are Now
[1-2 sentence honest summary: pipeline state, biggest gap, what's blocking revenue right now]

## 90-Day Revenue Target: $[X]
## Deals needed at $[avg deal size]: [#]
## Meetings needed (at [close rate]% close): [#]
## Prospects needed (at [meeting rate]% meeting rate): [#]
## Outreach volume needed (at [reply rate]% reply): [#/week]

## Aggressive 12-Week Roadmap
*Assumes dedicated sales focus. Adjust outreach volume targets if part-time.*

Week 1 — Foundation
  Goal: ICP locked, messaging built, sequences written
  - [ ] ICP definition stress-tested — specific enough that 2 reps target the same companies
  - [ ] Value proposition: one-sentence + one-paragraph + elevator pitch
  - [ ] Competitive positioning documented (vs. 3 most likely alternatives)
  - [ ] Messaging brief: 3 hook angles + 3 problem framings + proof point
  - [ ] Cold email sequence drafted (4-email, 2 subject line variants per email)
  - [ ] LinkedIn sequence drafted (connection + 3 DMs)
  - [ ] Objection map: top 5 objections + responses
  - [ ] CRM set up with pipeline stages and entry/exit criteria

Week 2 — Launch
  Goal: First outreach sent, system working
  - [ ] Prospect list #1 built: 100 companies matching ICP
  - [ ] Email domain warmed (if new domain — use a warm-up tool)
  - [ ] First 25 cold emails sent
  - [ ] First 25 LinkedIn connection requests sent
  - [ ] Tracking in place: open rate, reply rate, meetings per channel
  - [ ] PIPELINE_TRACKER.md updated daily

Week 3 — Volume
  Goal: Full sending cadence established
  - [ ] 50+ cold emails/week cadence established
  - [ ] 50+ LinkedIn touches/week cadence established
  - [ ] First replies coming in — qualify or disqualify each
  - [ ] Sequence follow-ups executing automatically
  - [ ] If open rate < 30%: test 3 new subject lines
  - [ ] If reply rate < 2%: rewrite email 1 with a different hook

Week 4 — First Meetings
  Goal: Discovery calls booked and run
  - [ ] 3+ discovery calls booked from outreach
  - [ ] Discovery call framework built (questions, timing, qualification criteria, next step)
  - [ ] Post-call: qualified or disqualified — documented in PIPELINE_TRACKER.md
  - [ ] Proposal template built from FLOW A step 6 (if not already)
  - [ ] Outreach at 200 total touches sent

Week 5 — Qualify and Refine
  Goal: Pipeline validated, messaging sharpened from real conversations
  - [ ] 5+ discovery calls completed
  - [ ] Common objections logged and added to objection map
  - [ ] ICP refined based on who's engaging vs. who isn't
  - [ ] Sequence variant B tested (different angle) on new prospect batch
  - [ ] 1-2 proposals sent

Week 6 — First Close Attempt
  Goal: First deal in final stage or closed
  - [ ] 1+ proposals in negotiation
  - [ ] Follow-up cadence on proposals (Day 2, Day 5, Day 10)
  - [ ] If deals stalling: identify the real objection, address directly
  - [ ] Referral ask from warm contacts: "Who else do you know who has [specific problem]?"
  - [ ] Outreach at 400 total touches sent

Week 7 — Scale What's Working
  Goal: Double down on the channel and message that's converting
  - [ ] Analyze: which channel has the best reply-to-meeting rate?
  - [ ] Which hook/subject line is outperforming? Standardize it.
  - [ ] Prospect list #2 built: 100 more ICP-matched companies
  - [ ] Volume increased on the winning channel by 50%
  - [ ] First client signed (if not yet: diagnose the specific blocker)

Week 8 — Pipeline Density
  Goal: Enough pipeline to guarantee target close
  - [ ] 10+ active prospects across pipeline stages
  - [ ] 3+ proposals sent or in progress
  - [ ] Referral program defined: what do you ask, when do you ask it, what's the incentive
  - [ ] First closed client: kickoff sent, onboarding started
  - [ ] Testimonial/case study drafted from first win (even if deal not fully complete)

Week 9 — Content Engine (Optional but high-leverage)
  Goal: Inbound signals start appearing
  - [ ] LinkedIn content: 3 posts/week minimum (problem-aware content for ICP)
  - [ ] First case study published (LinkedIn + website if applicable)
  - [ ] Partnership outreach: 10 non-competing companies serving same ICP
  - [ ] Outreach at 700 total touches sent

Week 10 — Systematize
  Goal: Sales process documented so it can scale beyond one person
  - [ ] Full sales playbook written: ICP, messaging, sequences, objection handling, discovery, proposal
  - [ ] Handoff process defined: sales → delivery → account management
  - [ ] Onboarding checklist finalized from first client experience
  - [ ] Renewal/expansion process defined: when to upsell, how, what triggers it

Week 11 — Acceleration
  Goal: Multiple deals closing in parallel
  - [ ] 3+ deals in negotiation simultaneously
  - [ ] Outreach volume maintained even while closing (pipeline never pauses)
  - [ ] Second case study published
  - [ ] LinkedIn profile updated to reflect wins
  - [ ] Referrals starting to come in from first client

Week 12 — 90-Day Review
  Goal: Honest assessment, next 90-day plan
  - [ ] Revenue target: hit / missed by [X]% / exceeded
  - [ ] Funnel metrics: where did deals stall? Which stage had lowest conversion?
  - [ ] Best channel: [channel] at [reply rate]% → double down
  - [ ] Worst channel: [channel] — pause or retest with new message
  - [ ] ICP accuracy: did ideal clients actually buy? Any surprises?
  - [ ] Next 90 days: [specific goal] — scale, expand ICP, or enter new channel

Beyond 90 Days:
  - Inbound content compounds as case studies and posts accumulate
  - Referral engine activates as client base grows
  - Partnership channel opens as trust is established with adjacent companies
  - Pricing increases quarterly as proof and demand compound
  - Enterprise motion begins once SMB playbook is repeatable
```

---

## Templates to scaffold

### Proposal (`outputs/proposals/proposal-template.md`)

```
# Proposal — [Company Name]

Prepared for: [Name, Title, Company]
Date: [Date] | Valid until: [Date + 14 days]

> Send within 24 hours of discovery call. Never send cold.

## The Situation
[Their problem in their words. 2-3 sentences. Reference specific things they said.]

## The Outcome
[What they'll have when this is done — their metric, their language.]

## Our Approach
1. [Step 1]
2. [Step 2]
3. [Step 3]

## What's Included
- [Deliverable 1]
- [Deliverable 2]
- [Revisions: X rounds]
- [Timeline: Start → Milestone → Delivery]

## What's Not Included
- [Specific exclusion]
- [Specific exclusion]
Additional scope is quoted separately before starting.

## Investment
| | Amount | Due |
|--|--------|-----|
| Deposit (50%) | $[X] | Before work starts |
| Final payment (50%) | $[X] | On delivery |
| **Total** | **$[X]** | |

## What Others Say
"[Specific result, specific client type, specific timeframe]"
— [Name, Title, Company]

## Next Steps
1. Reply to confirm
2. We send contract + invoice within 24 hours
3. Work starts [date] once deposit is received

Valid until [date].

*Follow-up: Day 2, Day 5, Day 10. Delete before sending.*
```

---

## Session continuity rules

Every session in this folder:

**On start:** Read GTM.md, PIPELINE_TRACKER.md, PROJECT_STATE.md — understand current state before asking anything. Never ask the user to recap what happened before.

**During session:** When new prospect data comes in (replies, meetings, outcomes), update PIPELINE_TRACKER.md. When sequences need adjustment, update outputs/sequences/.

**On end:** Update PROJECT_STATE.md with what was done. Update ROADMAP.md to mark completed items. Note any decisions — messaging changes, ICP refinements, channel shifts — and why.

---

## What this skill does NOT do

- Send emails or LinkedIn messages (generates templates, team sends)
- Access CRM systems directly (user pulls data and shares it)
- Research individual prospects (user provides prospect details)
- Legal or contract advice (generates templates, lawyer reviews)
