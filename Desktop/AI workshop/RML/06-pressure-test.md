---
type: analysis
topic: Real Math League — Pressure Test
date: 2026-04-07
status: draft
version: 1
---

# Real Math League — Pressure Test

A critical analysis of the RML concept: what's strong, where the gaps are, and what needs resolving before launch.

---

## What's Strong

**The content concept is proven.**
Cuemath Studio already validated this — GPS, Honeycombs, Tiki-Taka generated real excitement. The difference is RML puts that on the Cuemath domain with a conversion path. That's the right move.

**The PLG model is correct.**
No signup to start, full value before the gate. Most edtech gets this wrong by requiring signup upfront. RML gets it right.

**The SEO/AEO play is underrated.**
100 indexable pages on cuemath.com around queries like "why are honeycombs hexagons math" is genuinely valuable and compounds over time. This benefit isn't highlighted enough in the existing docs — it may be one of the strongest long-term returns from the project.

**The cardinal rules are the right constraints.**
Never intimidating, never boring, never traditional — if held ruthlessly, these three produce something genuinely different from everything else in the market. They need to be treated as veto criteria, not aspirations.

---

## The Gaps — In Order of Severity

---

### Gap 1 — The Conversion Path Has a Structural Hole *(Critical)*

This is the biggest risk and it's not fully addressed in the existing documents.

The person who loves RML is a child. The person who buys tutoring is a parent. These are different people with different motivations. The child does RML for curiosity and fun. The parent buys tutoring because of academic anxiety — fear of falling behind, exam pressure, competitive peers.

A child enjoying real-world math explorations does not naturally create parental purchase intent. In fact, a parent watching their child happily explore "why pizzas are weird math" may think: *great, Cuemath has a free thing, I don't need to pay.*

The parent email is the bridge designed to solve this — but it has three problems:
1. It requires a parent email at signup, which children often skip or enter incorrectly
2. It's a weekly digest, which is passive — it tells the parent their child is doing well, not that they need to do more
3. The nudge copy ("Want to take their math journey further?") is generic and doesn't create urgency

**What's missing:** The child's success on RML needs to be translated into a specific gap the parent can act on — not just general admiration. The difference between "Your child is doing great on RML" and "Your child scored in the top 10% on probability challenges but hasn't explored algebra — that's the gap that typically shows up in 7th grade" is the difference between a feel-good update and a conversion trigger. The latter creates a specific, actionable concern. The former doesn't.

**What needs to happen before launch:** Design a sharper parent-facing signal. Not just "your child is doing well" — but a specific insight about what they're strong at, what gap exists, and why it matters. This is the mechanism that justifies the tutoring nudge.

---

### Gap 2 — The Growth Projections Are Very Optimistic *(High)*

1M MAU in 12 months is the target. The ramp:

Month 1: 5K → Month 3: 40K → Month 6: 200K → Month 12: 1M

This assumes viral loops kick in aggressively from month 3 and school adoption compounds rapidly. That's possible — but it's the best case, not the base case. In edtech specifically:

- **Share rates on educational content are historically 2–5%**, not the 10–15% projected. Share cards work when the content is genuinely surprising — and some RML challenges will be. But the average across 100 challenges will be lower than the best.
- **School adoption is slow.** Teachers are overworked. "500 schools in 3 months" requires significant active outreach or organic teacher-to-teacher word-of-mouth, which typically takes 6+ months to develop.
- **SEO takes 6–12 months to compound.** It won't drive significant traffic in the first 3 months, regardless of content quality.

**A more realistic 12-month scenario is 150–250K MAU, not 1M.**

**What needs to happen before launch:** Stress-test the business case at 200K MAU. The revenue model built on 1M MAU projects $8.4M incremental revenue. At 200K MAU, that's approximately $1.7M. Is the investment still justified at that number? If yes — great, the upside case is a bonus. If no — the model needs rethinking.

| MAU Scenario | Tutoring Trials (1% CTR) | New Paid Students (35% conv) | Incremental Revenue ($2,400 LTV) |
|---|---|---|---|
| 1M (target) | 10,000 | 3,500 | $8.4M |
| 500K (realistic upside) | 5,000 | 1,750 | $4.2M |
| 200K (realistic base) | 2,000 | 700 | $1.7M |
| 100K (conservative) | 1,000 | 350 | $840K |

The investment case should be validated at the 200K scenario, not just the 1M scenario.

---

### Gap 3 — Habit Design Is Thin *(High)*

Duolingo's power comes from one thing: the streak. Users with a 7-day streak are 3.6x more likely to stay. The streak creates daily pull — you return not because you're curious but because you don't want to break it.

RML's current progression system has streaks — but they're secondary to the challenge model. A challenge takes 15–30 minutes and is discrete. You complete it, share it, and then make a new choice. There is no micro-action you can do in 3 minutes to keep the streak alive on a busy day.

This is a design gap. The DAU/MAU target of 20% is very hard to hit without a daily micro-engagement mechanic. Most challenge-based platforms see 5–8% DAU/MAU, not 20%.

**What needs to happen before launch:** Define the micro-action that keeps the streak alive. Options:
- A daily "Quick Explore" — one question from a challenge, 2–3 minutes, counts as activity
- A daily "Math Moment" — one surprising real-world math fact, with a reaction (like/think/share), keeps the streak
- Progress on a multi-session challenge counts as daily activity (challenges that take 3–5 days to complete, not 15 minutes)

The right mechanic needs to be designed and tested — not left as "streaks exist."

---

### Gap 4 — Desktop-First for an Audience That Lives on Phones *(High)*

The target audience is grades 3–10, ages 8–15. This demographic is overwhelmingly on mobile. "Desktop-first but fully functional on mobile" means the primary design decisions are made for a device most target users won't use.

The 15–30 minute challenge format also doesn't fit mobile usage patterns well. Mobile sessions are fragmented — 5–10 minutes, often interrupted. On mobile, text input, drag-and-drop, and estimation sliders all have meaningful friction.

This is a design question that needs an honest answer before building: **is the primary use case a kid at a computer, or a kid on a phone?** Desktop-first is a valid choice if the primary acquisition channel is schools (where kids use computers). It's the wrong choice if the primary acquisition channel is organic/social (where kids are on phones).

**What needs to happen before launch:** Align on primary device and design explicitly for it. If desktop-first is the choice, acknowledge that mobile conversion will be lower and factor that into projections. If mobile-first, the challenge format needs to be redesigned for shorter, interruptible sessions.

---

### Gap 5 — The Community Dimension Is Missing *(Medium)*

RML as designed is fundamentally a solo experience with social dressing. Leaderboards and share cards create competition and broadcasting — but not belonging.

A curious 12-year-old who completes "Why Democracy Needs Math" has nowhere to go with that insight. There's no one to argue with, no cohort who just discovered the same thing, no identity being formed. The share card goes to WhatsApp — to a general audience, not to people who care.

This is possibly a conscious trade-off: community is operationally complex and this is a lean launch. That's fine. But it means RML solves a different problem than community-based enrichment — it's a discovery and top-of-funnel engagement tool, not a belonging product. Being explicit about this shapes what success looks like and what the product roadmap looks like after launch.

**A future consideration:** Post-launch, a "league" layer that actually creates small cohorts of curious kids working through the same challenges simultaneously would be a natural evolution — and would dramatically increase retention. The name "Real Math League" implies this but the product doesn't deliver it yet.

---

### Gap 6 — Competitive Differentiation Is Underdeveloped *(Medium)*

The docs don't directly address existing players who are close to this space:

**Mathigon** (mathigon.org) — interactive, real-world math explorations with beautiful design. Free, well-regarded by math educators globally. The concept overlap with RML is significant. Differentiation needs to be explicit — Cuemath brand, school network, conversion path, and content style are the real wedges, but they need to be stated.

**Brilliant.org** — interactive STEM problem-solving, real-world contexts, progression system, $150/year subscription. $14–18M revenue. Overlaps at Level 5–7 for older students.

**NRICH** (Cambridge University) — free, real-world math problems, widely used in UK and international schools. Less polished but carries institutional trust.

None of these have Cuemath's distribution, brand, or conversion infrastructure. But teachers comparing free math tools will encounter them. Having a clear, one-line answer to "why RML and not Mathigon?" is worth preparing before school outreach begins.

---

### Gap 7 — Content Quality vs. Timeline Tension *(Medium)*

100 challenges in 6–8 weeks with a 4–5 person team. The math:

9 hours per challenge × 100 challenges = 900 hours of content work

Across 5 people over 7 weeks at full capacity: 5 × 7 × 40 = 1,400 hours total

That's 64% of total team capacity on content alone — before design, engineering, QA, school outreach, and launch coordination. It's doable but there's almost no slack. One challenge topic requiring more research than expected, one round of revision, one person at reduced capacity — and you're either late or you compromise quality.

The existing docs correctly note: "Better to launch with 70 great challenges than 100 mediocre ones." But this should be the plan, not the fallback. **Officially plan for 70 challenges at launch.** Use weeks 7–8 to add the remaining 30 only if quality holds. Protect the cardinal rules over the number.

---

### Gap 8 — The "Free Forever" Tension *(Medium)*

If RML is genuinely free forever and tutoring conversions are lower than projected, what's the case for continuing to invest? The business case rests entirely on the tutoring funnel. There's no explicit threshold in the existing documents.

The risk: RML becomes a beloved free product that costs real money to maintain (content creation, engineering, school outreach) but doesn't drive the tutoring funnel at the projected rate — and faces budget pressure without a clear decision framework.

**What needs to happen before launch:** Define explicit go/no-go metrics with a timeline. Example: "If we don't see 200 tutoring trials by month 3 post-launch, we review the conversion mechanism before continuing to invest in MAU growth." Without this, the team optimises for engagement (easy to show) rather than conversion (hard but what matters).

---

## Summary — What Needs Resolving Before Launch

| Gap | Severity | What needs to happen |
|---|---|---|
| **Conversion path** | Critical | Design a sharper parent-facing mechanism that creates specific, actionable concern — not just positive signal |
| **Growth projections** | High | Stress-test the business case at 200K MAU; validate investment at base case, not target case |
| **Habit design** | High | Define the micro-action that keeps the streak alive on a busy day — the 3-minute RML equivalent |
| **Device strategy** | High | Decide: desktop-first (school acquisition) or mobile-first (organic)? Build for one, not both |
| **Content timeline** | Medium | Plan for 70 challenges at launch; 100 is the upside, not the floor |
| **Free forever threshold** | Medium | Set explicit conversion milestones that trigger a review — protect against optimising for engagement over conversion |

The remaining gaps (community, competition) are real but manageable post-launch. The six above are pre-launch decisions.

---

## The One Question That Underlies Everything

**Is RML a brand play or a conversion play?**

If it's primarily a brand play — building love for Cuemath among kids and parents, establishing "excellence through wonder" as a position, generating SEO authority — then MAU is the right north star and conversion is a bonus. The investment is justified even if tutoring conversion is low, because the brand equity is real.

If it's primarily a conversion play — a zero-CAC channel to drive tutoring revenue — then conversion rate is the north star and MAU only matters insofar as it drives trials. The design decisions (parent nudge mechanism, conversion copy, trial booking flow) need to be sharper, and the go/no-go metrics need to be tied to revenue, not engagement.

The documents treat it as both simultaneously. That's fine for the pitch — but when making design trade-offs, the team needs to know which one wins. Clarity on this before launch prevents the wrong metrics from driving the wrong decisions.
