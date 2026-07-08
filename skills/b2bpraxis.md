# Skill: b2bpraxis

A B2B company growth system for Claude. Guides a company from ICP definition to repeatable revenue — outreach, content, lead magnets, and online presence all built around one core asset: the Blueprint. Sessions are persistent, state lives in files.

**Install:** Copy this file to `~/.claude/skills/b2bpraxis.md`
**Invoke:** `/b2bpraxis` in any company folder

---

## The Core Method — Blueprint First

Everything in this system is built around one insight: **send value before asking for anything.**

A Blueprint is not a pitch deck. It's a simple document that:
1. Names the problem your ICP is actively trying to solve
2. Shows the exact workflow to solve it (manually, step by step)
3. Shows proof: the result you got for a real client
4. Shows how the reader can replicate it themselves
5. Shows where your service/product makes it 10x faster

The Blueprint is the cold outreach hook, the LinkedIn lead magnet, the website opt-in, and the thing that makes strangers trust you before they've spoken to anyone on your team.

Once the Blueprint is built, everything else becomes distribution.

---

## On invoke — detect which flow to run

Check the current folder for:
- `GTM.md` or `PIPELINE_TRACKER.md` → existing operation, run FLOW B
- `outputs/` with any files → existing assets, run FLOW B
- Neither → new start, run FLOW A

Tell the user which flow you're running and why in one line.

---

## FLOW A — New B2B Operation

### Step 1: Clarity interview — ask all 9 in one message

```
1. What does your company sell, and what's the #1 outcome you deliver for clients?
   (e.g. "We cut SaaS churn by 30% using behavioral email automation")

2. Describe your ideal customer profile (ICP) as specifically as possible:
   Industry / company size / revenue range / title of buyer / title of user

3. What's your single strongest client result? (specific numbers, specific timeframe)

4. What's your average deal size and typical sales cycle length?

5. How are you currently generating leads? (inbound, outbound, referrals, partnerships — be specific)

6. What channels do you want to use?
   Cold email / LinkedIn / Cold calling / Reddit / YouTube / Events / Partnerships

7. Do you have a website? If yes, what's on it currently?

8. What's your revenue target for the next 90 days?

9. What is explicitly NOT in scope for now?
   (scope lock — prevents spreading effort too thin)
```

Wait for all 9 answers before proceeding.

### Step 2: ICP stress test

Before building anything, pressure-test the ICP and value proposition:

- **Pain test:** Does the problem you solve cause companies to actively spend money trying to fix it right now?
- **Specificity test:** If you showed your ICP definition to 10 reps, would they all target the same kind of company?
- **Proof test:** Do you have at least 1 client who got the result you're promising, with a number attached?
- **Blueprint test:** Can you describe the workflow your service delivers as a step-by-step process someone could follow manually? If not, the offer isn't specific enough yet.
- **"Why you" test:** Why would this ICP choose you over an alternative? Name the real differentiator.

Give a verdict: ✅ STRONG / ⚠️ REFINE / 🔄 REFRAME. Fix before continuing.

### Step 3: Build the Blueprint (the core asset — build this first)

The Blueprint is built before any sequence, post, or page. Everything else is just distribution of this document.

Generate and save to `outputs/blueprint.md`:

```
# [Company Name] Blueprint: [Specific outcome the ICP wants]

## The Problem
[2-3 sentences. Describe the specific pain your ICP feels. Use their language.
Make them think "this person gets it."]

## The Manual Workflow (step by step)
Here's how to [achieve the outcome] without any tools:

Step 1: [Specific action — e.g. "Find LinkedIn posts where your ICP is asking about [problem]"]
Step 2: [Specific action]
Step 3: [Specific action]
Step 4: [Specific action]
Step 5: [Specific action]

[Include where to find things, what to look for, how to qualify — real operational detail]

## The Proof
We used this exact workflow for [client type].
Result: [specific metric] in [specific timeframe].

[One sentence of context on the client's situation before they worked with you]
[One sentence on what changed after]

## How to Make This 10x Faster
The manual process above works. It's just slow.

Here's where [Your Company] speeds it up:
- [Step 1 manual → how your service handles it]
- [Step 2 manual → how your service handles it]
- [Step 3 manual → how your service handles it]

[Screenshot or description of the result in your system if applicable]

## Get Started
[CTA — NOT "book a demo." Options:]
- "Reply YES and we'll set this up for your specific market"
- "Start a free trial at [URL]"
- "Book a 20-minute setup call — we'll walk through your exact ICP" [link]

---
*[Your Company] | [website] | [one-line what you do]*
```

After generating: confirm the proof point is real and the workflow is specific enough. If the workflow is vague, push the user to make it operational.

### Step 4: Scaffold the operation

Generate these files:

**GTM.md** — go-to-market spec covering:
- ICP definition (industry, size, revenue, buyer title, user title, trigger events)
- Value proposition: one sentence, one paragraph, elevator pitch
- Competitive positioning: how you're different from the 3 most likely alternatives
- Pricing tiers and deal structure
- Sales process stages with entry/exit criteria per stage
- Objection map: top 5 objections + how to handle each
- Blueprint distribution: which channels get the blueprint and how

**PIPELINE_TRACKER.md** — copy from templates/PIPELINE_TRACKER.md, populate with ICP and goals

**CONTENT_TRACKER.md** — copy from templates/CONTENT_TRACKER.md (scaffold this too)

**PROJECT_STATE.md** — starting state:
- Date started, ICP confirmed, channels selected, 90-day revenue target
- Blueprint: built / not built
- What's next: outreach sequences → website lead magnet page → LinkedIn content

**ROADMAP.md** — generate the 12-week roadmap (see Roadmap section below)

**CLAUDE.md** — scaffold with these session rules:
```
At START of every session:
  Read GTM.md — ICP, positioning, objection map
  Read PIPELINE_TRACKER.md — current pipeline state
  Read CONTENT_TRACKER.md — content performance, what's published
  Read PROJECT_STATE.md — where we left off
  Read ROADMAP.md — what's due this week

At END of every session:
  Update PIPELINE_TRACKER.md with replies, stage changes, closed deals
  Update CONTENT_TRACKER.md with new posts, performance data
  Update PROJECT_STATE.md: what was done, decisions made and why
  Update ROADMAP.md: mark completed items, flag slippage
  Save new assets to outputs/
```

### Step 5: Build outreach sequences — Blueprint method

**The rule:** Never ask for a demo in the first touch. Send the blueprint instead. The blueprint sells. The demo ask lives inside the blueprint.

**Cold email sequence** (`outputs/sequences/cold-email.md`):

```
Email 1 — Day 1: Blueprint offer (not a demo ask)
Subject A: "How [similar company type] got [specific result]"
Subject B: "[First name] — the [specific workflow] we used for [client type]"
Subject C: "Quick question about [specific pain they likely have]"

Body:
Hi [Name],

[One sentence showing you know who they are and what they care about — not flattery, relevance]

We helped [similar company type] [specific result] in [timeframe] using [brief description of method].

I wrote up the exact workflow — [specific outcome it shows them how to achieve].

Want me to send it over? Just reply YES.

[Name]
[Title] at [Company]

---

Email 2 — Day 3: Follow-up if no reply
Subject: "Re: [same thread]"

Body:
Sending this in case it landed wrong.

The doc I mentioned shows [specific step of the workflow] — the part most [ICP title] get stuck on.

Still happy to send it. Just reply YES.

---

Email 3 — Day 7: Different angle
Subject: "[Specific pain point]?"

Body:
Quick question — is [specific problem] something you're actively working on?

[One sentence social proof — who else in their space had this problem and what changed]

Happy to send the workflow doc if useful. Or not — no pressure either way.

---

Email 4 — Day 14: Break-up
Subject: "Closing the loop"

Body:
I'll stop reaching out after this one.

If [specific pain] ever becomes a priority, the workflow doc is available whenever.

[Name]
```

**LinkedIn sequence** (`outputs/sequences/linkedin.md`):

```
Connection request (300 chars max):
"[Name] — I write about [their topic of interest] and saw your post on [specific thing].
Connecting to share a workflow doc on [relevant topic] if useful."

DM 1 — Day 2 after connect:
"Thanks for connecting, [Name]. I promised a doc on [topic].
Here's the workflow we used to [specific result] — [link or paste blueprint].
No CTA, just the method. Happy to talk through the setup if useful."

DM 2 — Day 5 (if no reply to DM 1):
"[Name] — just checking this landed. The doc covers [specific step] which I know [their role]
usually handles manually. Let me know if you want to talk through applying it."

DM 3 — Day 10:
"Last one from me. If [specific pain] is ever a priority, reach out — happy to help."
```

**Cold call script** (`outputs/sequences/cold-call.md`) if selected:
- Opening (5 sec): name + company + permission
- Bridge (10 sec): "I sent you a doc about [specific outcome] — did it land?"
  (If haven't emailed yet: "I help [ICP type] [specific result] — is that something you're working on right now?")
- Value statement (10 sec): result for similar company
- Qualifying question: get them talking about the problem
- Objection handlers for top 3
- CTA: send blueprint, book setup call, or next step

### Step 6: Build the content engine

Content is Blueprint distribution. Every post, video, and article is an excerpt or angle from the Blueprint.

**LinkedIn content plan** (`outputs/content/linkedin-plan.md`):

Post cadence: 6 lead magnet posts per week + 1 founder/behind-the-scenes post

Lead magnet post formats (rotate):
```
Format 1 — Step from the workflow
"Most [ICP role] [do X wrong]. Here's the right way:
[Step 1] ...
[Step 2] ...
[Full workflow in comments — drop a ✅ and I'll send the doc]"

Format 2 — Proof post
"We helped [client type] go from [before] to [after] in [timeframe].
Here's exactly what we did: [3-4 step summary]
The full breakdown is in a doc I put together. Reply ✅ if you want it."

Format 3 — Contrarian take
"[Common belief in ICP's world] is wrong.
Here's what actually works: [your method]
[Specific result to back it up]
Comment [keyword] and I'll send the full process."

Format 4 — Before/after
"Before working with us: [specific pain point with number]
After: [specific result with number]
The process that made the difference: [2-3 sentences]
Full breakdown → comment YES"

Format 5 — Direct question
"[ICP role]: are you still [doing painful manual thing]?
We automated this for [client type]. Takes [X minutes] instead of [Y hours].
Here's how: [link to blueprint or comment trigger]"

Format 6 — Insight
"[Non-obvious insight about ICP's problem].
Most people miss [X] because [Y].
The fix: [Z — excerpt from blueprint workflow]
Full doc in comments if useful."

Founder day (1 per week):
"What we shipped this week / what I learned / behind the scenes / honest update"
```

**Comment automation note:**
Set up a LinkedIn automation tool to reply to any comment with the trigger word (✅, YES, keyword) with a direct message containing the Blueprint link. This turns every post into a passive lead gen machine. The tool detects the comment and DMs the Blueprint automatically. Popular tools: MeetAlfred, Phantombuster (use responsibly within platform limits).

**Reddit strategy** (`outputs/content/reddit-plan.md`):

High-value subreddits for B2B companies (one post can drive 5,000+ visitors):

```
Primary targets (post here first):
r/SaaS (~500K) — for SaaS companies
r/Entrepreneur (~5M) — broad business audience
r/startups (~2M) — startup-focused
r/smallbusiness (~2.3M) — SMB-focused
r/EntrepreneurRideAlong (~640K) — build-in-public friendly

Secondary targets (rotate in):
r/indiehackers (~143K)
r/SideProject (~580K)
r/marketing / r/digitalmarketing / r/growthhacking
r/SEO / r/webdev / r/programming (if relevant)
r/consulting / r/freelance (if service-based)
r/Business_Ideas / r/startup_ideas (for early validation)
r/RoastMyStartup (for feedback loops)
```

Reddit post rules:
- Lead with value, not promotion. The post is the content. The company is mentioned at the end, if at all.
- "Here's the exact process we used to [specific result]" outperforms "Check out our tool."
- Share the manual workflow from the Blueprint as the Reddit post. The comments will ask how to do it faster — that's when you mention the company.
- 2 posts/week minimum. Test which subreddit drives actual traffic (UTM links on Blueprint URL).

**YouTube strategy** (`outputs/content/youtube-plan.md`):

Strategy: rank on competitor keywords + ICP problem keywords (SEO-first, not viral-first)

Video types that work:
```
Type 1 — Tutorial (highest search volume)
"How to [achieve the outcome from your Blueprint] — step by step"
Structure: problem (30s) → why most people fail (60s) → the correct workflow (4-6 min) → where to learn more (30s)

Type 2 — Competitor comparison
"[Competitor] vs [Your Company] — honest breakdown"
"Why we switched from [Competitor] to [this approach]"

Type 3 — Case study walkthrough
"How [client type] went from [before] to [after] — the exact process"

Type 4 — Build-in-public
"[Month] update: what's working and what's not"
"How we got our first [X] customers without paid ads"
```

Frequency: 1-2 per week is enough if the videos rank. Quality over volume. Optimize title and description for search.

**Twitter/X strategy** (`outputs/content/twitter-plan.md`):

3 posts per day, no strict strategy. Document what you're building:
- Metrics updates ("We hit [X] this week. Here's what worked.")
- Lessons from client work
- Contrarian takes on the industry
- Reposts of LinkedIn content (different audience, low effort)
- Engage with ICP-adjacent accounts (reply to their posts with useful insight)

### Step 7: Build the website lead magnet page

If the company has a website (or plans to build one), the Blueprint becomes the primary opt-in offer.

Generate `outputs/website/lead-magnet-page.md`:

```
# Lead Magnet Page Brief

URL: /free-blueprint (or /[keyword]-guide, /[specific-outcome]-framework)

Above the fold:
  Headline: "The [specific outcome] Blueprint: [how to achieve it] without [specific pain]"
  Subheadline: "The exact workflow we used to [specific result] for [client type] — free"
  CTA: [Email field] + "Send me the Blueprint"
  Trust element: "[# companies] have downloaded this" or "[client name] used this to [result]"

Below the fold (keep it short — this is a lead gen page, not a content page):
  What's inside (3-4 bullets): specific, outcome-focused
  One testimonial: from someone who used the workflow
  Repeat CTA

After opt-in:
  Redirect to thank-you page with immediate Blueprint access
  Add to email sequence: Day 1 (Blueprint delivered) → Day 3 (follow-up: did it help?) →
  Day 7 (case study) → Day 14 (offer: book a call or start trial)

Traffic sources for this page:
  - LinkedIn posts with "comment YES" → DM with link → drives to this page
  - Cold email sequence (Blueprint sent directly, not gated — removes friction)
  - Reddit posts linking here
  - YouTube video descriptions
  - Paid retargeting (later, once organic is converting)
```

### Step 8: Confirmation gate

Present Blueprint, sequences, content plan, and lead magnet page brief. Wait for confirmation before anything goes out or gets published.

---

## FLOW B — Existing B2B Operation

### Step 1: Audit the current state

Ask the user to share:
- Any existing sequences or outreach templates
- Current pipeline: how many prospects at each stage
- Existing content: what's been published, which channels, performance metrics
- Website: does it have a lead magnet or opt-in? What's the opt-in rate?
- Last 3 clients won: how they came in, how long the cycle was
- Biggest blocker: outreach volume, reply rate, content traction, or closing

### Step 2: Diagnose the revenue and visibility gap

Map both the funnel AND the content engine:

```
## Revenue Funnel Audit
Outreach volume: [#/week] → Is this enough to hit target?
Open rate: [X]% → Benchmark: >40%
Reply rate: [X]% → Benchmark: >5% cold
Meeting rate: [X]% of replies → Benchmark: >40%
Close rate: [X]% of meetings → Benchmark: >25%

## Content & Lead Magnet Audit
Blueprint exists: Yes / No (if No: build this first)
LinkedIn posts/week: [#] → Benchmark: 5+ for meaningful reach
Lead magnet on website: Yes / No → Opt-in rate if yes: [X]%
Reddit posts: [#/month]
YouTube: [#] videos, avg views: [#]
Inbound from content: [#] leads/month

## Combined Diagnosis
[Single sentence: is the biggest gap outreach volume, message quality, or content/inbound visibility?]
```

### Step 3: Assess existing assets

- **Blueprint:** Does one exist? Is it specific (workflow with steps) or generic (company overview)?
- **Sequences:** Do they lead with the blueprint or ask for a demo in Email 1?
- **LinkedIn:** Is it lead magnet content or just company updates and reposts?
- **Website:** Is there a dedicated lead magnet page with an email opt-in?
- **Reddit/YouTube:** Presence or not?

Flag what needs to be built vs. what already works.

### Step 4: Scaffold missing files

Create any of these that don't exist:
- GTM.md, PIPELINE_TRACKER.md, CONTENT_TRACKER.md, PROJECT_STATE.md, CLAUDE.md, ROADMAP.md

Start roadmap from wherever they actually are — mark completed weeks done.

---

## Roadmap — 12-Week Aggressive B2B Growth

Outreach + content + lead magnets run in parallel from Week 2 onward. The Blueprint unlocks all three.

```
## Where You Are Now
[1-2 sentence honest summary: pipeline state, content presence, biggest gap]

## 90-Day Target: $[X] revenue + [#] inbound leads/month from content
## Deals needed: [#] | Meetings needed: [#] | Outreach volume: [#/week]

Week 1 — Foundation
  Goal: Blueprint built, ICP locked, operation scaffolded
  - [ ] ICP stress-tested — specific enough that 2 reps target the same companies
  - [ ] Blueprint built: problem + workflow + proof + 10x faster section + CTA
  - [ ] Value proposition: one-sentence + one-paragraph + elevator pitch
  - [ ] Competitive positioning documented (vs. 3 most likely alternatives)
  - [ ] Objection map: top 5 objections + responses
  - [ ] CRM set up with pipeline stages

Week 2 — Launch Outreach + Content Simultaneously
  Goal: First outreach sent, first content published, Blueprint live on website
  - [ ] Cold email sequence written (Blueprint method — reply YES, not book a demo)
  - [ ] LinkedIn sequence written (Blueprint in DM 1)
  - [ ] First 25 cold emails sent (Blueprint offer)
  - [ ] First 25 LinkedIn connection requests sent
  - [ ] LinkedIn post #1 published (lead magnet format — workflow excerpt)
  - [ ] Website lead magnet page live (Blueprint as opt-in)
  - [ ] Reddit post #1 published (manual workflow, no pitch)

Week 3 — Volume + Content Cadence
  Goal: Full sending cadence established, LinkedIn momentum building
  - [ ] 50+ cold emails/week cadence
  - [ ] 50+ LinkedIn touches/week
  - [ ] LinkedIn: 5 posts published this week (4 lead magnet, 1 founder)
  - [ ] Comment automation set up: trigger word → DM with Blueprint link
  - [ ] Reddit post #2 published
  - [ ] First replies coming in — qualify or disqualify
  - [ ] If open rate < 30%: test 3 new subject lines
  - [ ] If reply rate < 2%: rewrite Email 1 (different hook, same Blueprint offer)

Week 4 — First Meetings + First Inbound
  Goal: Discovery calls booked, first opt-ins from content
  - [ ] 3+ discovery calls booked from outreach
  - [ ] Discovery call framework built
  - [ ] Website lead magnet page: first email opt-ins coming in
  - [ ] LinkedIn: 5 posts, track which format drives the most comment/DM responses
  - [ ] YouTube: first video uploaded (Blueprint walkthrough — "how to [outcome]")
  - [ ] Outreach at 200 total touches

Week 5 — Qualify and Content Traction
  Goal: Pipeline validated, content formats identified
  - [ ] 5+ discovery calls completed, common objections logged
  - [ ] 1-2 proposals sent
  - [ ] Best LinkedIn post format identified — double down on it
  - [ ] Reddit post driving traffic? (check UTM on Blueprint page link)
  - [ ] YouTube: second video published (case study walkthrough)
  - [ ] Email list from Blueprint opt-ins: first nurture email sent

Week 6 — First Close + Content Compounding
  Goal: First deal closed or in final stage, content generating inbound
  - [ ] 1+ proposals in negotiation
  - [ ] Follow-up cadence on proposals (Day 2, Day 5, Day 10)
  - [ ] LinkedIn: first post breaking 1,000 impressions — analyze why
  - [ ] Blueprint opt-in email sequence: Day 7 email sent to list
  - [ ] Reddit: best-performing post identified — post similar content in 2 new subreddits
  - [ ] Outreach at 400 total touches

Week 7 — Scale What's Working
  Goal: Double down on the channel with best ROI
  - [ ] Analyze: which channel (cold email / LinkedIn DM / Reddit / YouTube) driving meetings?
  - [ ] Prospect list #2: 100 more ICP-matched companies
  - [ ] Volume increased 50% on winning outreach channel
  - [ ] Content: 1 new lead magnet format tested (different angle on same Blueprint)
  - [ ] Website lead magnet: A/B test headline if opt-in rate < 15%
  - [ ] First client signed (if not yet: diagnose blocker)

Week 8 — Pipeline Density + Authority Building
  Goal: Multiple deals in progress, content-driven inbound increasing
  - [ ] 10+ active prospects across stages
  - [ ] 3+ proposals sent or in progress
  - [ ] First case study published (LinkedIn long-form + YouTube video)
  - [ ] Blueprint v2: updated with proof from first closed deal
  - [ ] Email list: 50+ opt-ins — send case study to full list
  - [ ] Referral program defined: when to ask, what to offer

Week 9 — Content Engine at Full Speed
  Goal: Inbound leads arriving weekly from content
  - [ ] LinkedIn: consistent 5 posts/week, 3+ posts over 5,000 impressions
  - [ ] Reddit: 2 posts/week, at least 1 post drove 500+ visitors to site
  - [ ] YouTube: 3 videos live, at least 1 ranking on target keyword
  - [ ] Blueprint page: 25+ email opt-ins/month
  - [ ] Partnership outreach: 10 non-competing companies serving same ICP
  - [ ] Outreach at 700 total touches

Week 10 — Systematize
  Goal: Sales process and content engine documented for delegation
  - [ ] Full sales playbook: ICP, Blueprint, sequences, objection handling, discovery, proposal
  - [ ] Content playbook: which formats work, post cadence, subreddits, video topics
  - [ ] Onboarding checklist finalized from first client
  - [ ] Renewal/expansion process defined

Week 11 — Acceleration
  Goal: Multiple deals closing + consistent inbound
  - [ ] 3+ deals in negotiation simultaneously
  - [ ] Outreach volume maintained even while closing
  - [ ] Second case study published
  - [ ] Blueprint opt-in email list: 100+ subscribers, weekly email going out
  - [ ] First referral from existing client

Week 12 — 90-Day Review
  Goal: Honest assessment, next 90-day plan
  - [ ] Revenue: hit / missed by [X]% / exceeded
  - [ ] Best outreach channel: [channel] at [reply rate]%
  - [ ] Best content channel: [channel] driving [#] inbound leads/month
  - [ ] Blueprint opt-in rate: [X]% — does it need a new hook?
  - [ ] ICP accuracy: did ideal clients buy? Any surprises?
  - [ ] Next 90 days: [specific goal — scale, new ICP, enterprise motion, paid ads]

Beyond 90 Days:
  - Content compounds: old posts and videos keep generating opt-ins
  - Blueprint v3+: updated with more proof, better workflow
  - Paid retargeting to Blueprint page (warm traffic, much cheaper CPL)
  - Enterprise motion: Blueprint becomes a sales tool for larger deals
  - Partnership channel: joint blueprints with complementary companies
```

---

## Templates to scaffold

### Blueprint (`outputs/blueprint.md`) — see Step 3

### Proposal (`outputs/proposals/proposal-template.md`)

```
# Proposal — [Company Name]

Prepared for: [Name, Title, Company]
Date: [Date] | Valid until: [Date + 14 days]

> Send within 24 hours of discovery call. Never send cold.

## The Situation
[Their problem in their words. 2-3 sentences. Reference specific things they said on the call.]

## The Outcome
[What they'll have when this is done — their metric, their language, their timeframe.]

## Our Approach
1. [Step 1 from the workflow]
2. [Step 2]
3. [Step 3]

## What's Included
- [Deliverable 1]
- [Deliverable 2]
- [Timeline: Start → Milestone → Delivery]
Additional scope is quoted separately before starting.

## Investment
| | Amount | Due |
|--|--------|-----|
| Deposit (50%) | $[X] | Before work starts |
| Final (50%) | $[X] | On delivery |
| **Total** | **$[X]** | |

## What Others Say
"[Specific result, specific client type, specific timeframe]"
— [Name, Title, Company]

## Next Steps
1. Reply to confirm
2. Contract + invoice within 24 hours
3. Work starts [date] once deposit received

Valid until [date].
*Follow-up: Day 2, Day 5, Day 10. Delete before sending.*
```

---

## Session continuity rules

**On start:** Read GTM.md, PIPELINE_TRACKER.md, CONTENT_TRACKER.md, PROJECT_STATE.md. Never ask the user to recap.

**During session:** Update PIPELINE_TRACKER.md when deals move stages. Update CONTENT_TRACKER.md when posts go live or metrics come in. Flag if Blueprint needs updating based on new proof.

**On end:** Update PROJECT_STATE.md and ROADMAP.md. Save all new assets to outputs/.

---

## What this skill does NOT do

- Send emails or LinkedIn messages (generates templates, team sends)
- Access CRM or analytics directly (user shares data)
- Research individual prospects (user provides lists)
- Legal advice (generates templates, lawyer reviews)
- Publish to LinkedIn/Reddit/YouTube (generates content, team publishes)
