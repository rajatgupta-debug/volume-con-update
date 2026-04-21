---
type: plan
topic: Real Math League — Launch Plan
date: 2026-04-07
status: draft
version: 1
---

# Real Math League — Launch Plan

## Team

| Role | Person | Responsibilities |
|------|--------|-----------------|
| **Content Lead + Owner** | Karan | Overall RML ownership, content strategy, challenge quality, launch coordination |
| **Content Team** | Karan's team | Challenge creation using AI-assisted workflow, review and polish, theme research |
| **Designer** | TBD (1 person) | UI/UX design, design system, challenge illustrations, share card templates |
| **Frontend Dev** | TBD (1 person) | Web build on cuemath.com/league, using AI-assisted coding (Cursor/Copilot) |

**Total team: 4-5 people.** No dependency on core Cuemath engineering. This is a self-contained squad that builds, launches, and iterates independently.

### Why This Works Lean
- Content is AI-assisted — Karan's team uses AI to draft challenges, then reviews and polishes. Target velocity: 3-5 challenges/day per person.
- Frontend is AI-assisted — A single skilled dev using AI coding tools can build a Next.js app of this scope in 4-5 weeks.
- Design system, once established in Week 1, enables rapid challenge page creation without per-challenge design work.
- Simple backend needs (progress, leaderboard, auth) can use existing Cuemath infra or lightweight services.

## Week-by-Week Milestones

### Week 1 — Foundation

**Content:**
- Challenge template finalized (structure, step types, scoring rubric, metadata schema)
- 10 pilot challenges written across 3-4 themes
- Style guide for challenge writing: tone, length, visual direction per step

**Design:**
- Design system established: colors, typography, spacing, component library
- Challenge card component designed
- Homepage wireframe and high-fidelity mockup
- In-challenge step layout designed

**Engineering:**
- Next.js project scaffolded under cuemath.com/league
- Routing structure set up
- Challenge data model defined (JSON/MDX)
- Local development environment running

**Milestone check:** Can internally play through 10 challenges in a rough but functional UI.

---

### Week 2 — Content Velocity + Core Pages

**Content:**
- 30 challenges complete (20 new)
- All 10 themes represented
- Levels 1-7 all have at least 2 challenges each

**Design:**
- Challenge detail page designed
- Completion screen designed
- Share card template designed (2-3 variants)
- Leaderboard page wireframe

**Engineering:**
- Homepage built (hero, theme carousel, challenge grid)
- Challenge browsing page with filters functional
- Challenge detail page rendering from data
- Static share card generation (image export)

**Milestone check:** Can browse challenges on a real website and view detail pages.

---

### Week 3 — Core Experience Live

**Content:**
- 50 challenges complete (20 new)
- Quality review pass on all 50 — narrative flow, visual direction, scoring
- Challenge categorization and difficulty calibration

**Design:**
- In-challenge UI polish (all input types designed)
- Feedback states designed (correct, hint, explanation)
- Leaderboard page high-fidelity
- Profile page wireframe

**Engineering:**
- In-challenge step-by-step flow functional (all input types: MCQ, numeric, slider, text)
- Progress bar working
- Challenge completion flow end-to-end
- Leaderboard skeleton (UI + mock data)
- Basic scoring engine

**Milestone check:** Can browse, accept, complete a challenge, and see a completion screen. End-to-end flow works.

---

### Week 4 — PLG Flow + Social

**Content:**
- 70 challenges complete (20 new)
- Audio reasoning input tested on 5 challenges
- Challenge-a-friend copy and hooks written for all challenges

**Design:**
- Signup/login flow designed (minimal, fast)
- Profile page high-fidelity
- Mobile responsive pass on all pages
- Tutoring nudge designs (3 surfaces)

**Engineering:**
- Anonymous browsing → signup gate implemented
- Auth integration (Google + email, connect to Cuemath auth)
- Progress persistence (signed-in users)
- Share card generation and sharing (WhatsApp, Instagram, copy link)
- Challenge-a-friend deep links

**Milestone check:** Full PLG flow works: browse without signup → complete challenge → sign up to save → share card to WhatsApp.

---

### Week 5 — School Dashboard + Polish

**Content:**
- 85 challenges complete (15 new)
- Final review pass: consistency check across all challenges
- Teacher-facing content: "How to use RML in your classroom" guide

**Design:**
- Teacher dashboard designed
- Badges and achievements visual design
- Animation specs for completion screen
- Final polish pass on all pages

**Engineering:**
- Teacher dashboard MVP (class creation, join link, progress view)
- School leaderboard functional (real data)
- City and grade leaderboards
- Profile page with XP, level, badges, theme radar chart
- Performance optimization pass (Lighthouse audit)

**Milestone check:** A teacher can set up a class, students can join, teacher sees progress. Leaderboards populate with real data.

---

### Week 6 — Content Complete + QA

**Content:**
- 100 challenges complete (15 new)
- All challenges have: illustration direction, alt text, SEO content block
- Full coverage: every level (1-7) has 12-15 challenges, every theme has 8-12

**Design:**
- QA pass on all screens (desktop, tablet, mobile)
- Share card A/B variants finalized
- School outreach email template designed
- Social media assets for launch

**Engineering:**
- All 100 challenges loaded and playable
- QA: cross-browser testing (Chrome, Safari, Firefox, Edge)
- QA: mobile testing (iOS Safari, Android Chrome)
- Analytics integration: all events tracked
- SEO: meta tags, OG tags, structured data on all challenge pages
- Soft launch to internal team + 10 select schools

**Milestone check:** 100 challenges live, all features working, analytics flowing. Internal team and select schools actively using.

---

### Week 7 — Public Launch

**Content:**
- Bug fixes and content corrections from soft launch feedback
- 5 "hero" challenges identified for launch marketing

**Design:**
- Launch social media posts designed
- Press kit / media assets prepared

**Engineering:**
- Production deployment on cuemath.com/league
- CDN and caching optimized for traffic
- Monitoring and alerting set up
- Rate limiting and abuse prevention

**Launch activities:**
- Public announcement on Cuemath social channels
- School outreach campaign begins (email to target school list)
- Teacher community posts (Reddit, Facebook, forums)
- Internal Cuemath team shares with their networks
- Cuemath tutors share with students and parents

**Milestone check:** RML is live, public, and being used by real users outside Cuemath.

---

### Week 8 — Iteration

**Content:**
- 5-10 new challenges based on launch data (which themes are most popular?)
- Content quality improvements based on user behavior (where do users drop off?)

**Engineering:**
- Performance fixes based on real-world usage patterns
- UX improvements from user feedback
- A/B tests launched: signup gate timing, share card variants, nudge copy
- First conversion data: how many RML users book a tutoring trial?

**Analysis:**
- Week 1 post-launch metrics review
- Funnel analysis: visit → challenge start → completion → signup → share
- School adoption analysis: which outreach channels are working?
- First pass on tutoring conversion attribution

**Milestone check:** Data-informed iteration cycle is running. Team knows what's working and what needs fixing.

## Content Production Plan

### Challenge Template Structure

Each challenge is defined by a structured document:

```
Challenge metadata:
  - Title, slug, theme, level (1-7), estimated duration
  - Hook question (1 sentence teaser)
  - Key insight (the "aha" revealed at completion)
  - SEO description (150 chars)

Steps (5-12 per challenge):
  - Step type: context / question-mcq / question-numeric / question-slider / question-text / question-audio
  - Narrative text (2-3 sentences)
  - Visual direction (description for illustration/diagram)
  - Question (if applicable)
  - Answer + explanation
  - Scoring: points allocated per step
```

### AI-Assisted Writing Workflow

1. **Seed:** Team member identifies a real-world math topic and core insight
2. **Draft:** AI generates a full challenge draft from the seed (template-guided prompt)
3. **Review:** Team member reviews for accuracy, narrative flow, age-appropriateness, tone
4. **Visual direction:** Team member writes visual descriptions for each step (AI can assist)
5. **Polish:** Final language pass — does it sound like Cuemath? Is it never intimidating, never boring, never traditional?
6. **QA:** Different team member plays through the challenge end-to-end

**Target velocity:** 3-5 challenges per person per day at steady state (after template and workflow are refined in Week 1).

### Quality Review Checklist
- [ ] Math is accurate
- [ ] Narrative flows logically — each step builds on the previous
- [ ] Hook question is genuinely intriguing
- [ ] Key insight is satisfying and memorable
- [ ] Language is conversational, not textbook
- [ ] Appropriate for the target level (grade)
- [ ] Duration estimate is realistic (timed playthrough)
- [ ] Visual direction is clear and specific
- [ ] At least 2 different input types used
- [ ] No step feels like busywork
- [ ] Cardinal rules: not intimidating, not boring, not traditional

## Tech Stack

| Layer | Technology | Notes |
|-------|-----------|-------|
| **Frontend** | Next.js (React) | Deployed on cuemath.com/league as a route |
| **Styling** | Tailwind CSS | Rapid development, design system tokens |
| **Animations** | Framer Motion | Completion celebrations, micro-interactions |
| **Challenge data** | MDX or JSON | Static challenge content, no CMS needed at launch |
| **Auth** | Cuemath auth integration | Google + email signup, session management |
| **Backend API** | Node.js / Express (or Next.js API routes) | Progress tracking, leaderboard, XP |
| **Database** | PostgreSQL | User progress, scores, leaderboard data |
| **Image generation** | Canvas API / Sharp | Server-side share card rendering |
| **Analytics** | Mixpanel or Amplitude | Event tracking, funnel analysis |
| **Hosting** | Vercel or existing Cuemath infra | CDN, edge caching for challenge pages |
| **Audio** | Web Audio API + S3 | Audio recording, storage, playback |

## Launch Checklist

### Content
- [ ] 100 challenges complete and reviewed
- [ ] All themes and levels represented
- [ ] Challenge illustrations / visual direction finalized
- [ ] Share card copy written for all challenges
- [ ] SEO content blocks written for all challenge pages

### Tech
- [ ] All pages responsive (desktop, tablet, mobile)
- [ ] Cross-browser tested
- [ ] Performance: Lighthouse score > 90 on all pages
- [ ] Analytics: all events firing correctly
- [ ] Auth flow working (signup, login, session persistence)
- [ ] Share mechanics working (WhatsApp, Instagram, copy link)
- [ ] Leaderboard populating correctly
- [ ] Teacher dashboard functional
- [ ] Error handling and fallback states
- [ ] Rate limiting on API endpoints

### School Outreach
- [ ] Outreach email template written and designed
- [ ] Target school list compiled (start with Cuemath network)
- [ ] Teacher landing page live (/league/teachers/)
- [ ] "How to use RML in your classroom" guide ready
- [ ] Tutor ambassador instructions sent

### Analytics
- [ ] Event tracking validated end-to-end
- [ ] Funnel dashboards built (visit → start → complete → signup → share → trial)
- [ ] Leaderboard analytics (school activation, geographic spread)
- [ ] Conversion attribution set up (RML user → tutoring trial → paid)

### Tutoring Integration
- [ ] Post-challenge nudge live (shown after 2+ completions)
- [ ] Profile page nudge live
- [ ] Parent email flow set up (triggers after 1 week of activity)
- [ ] Trial booking link tracked with RML attribution

## Success Metrics

### 30 Days Post-Launch

| Metric | Target |
|--------|--------|
| MAU | 15K |
| Challenges completed | 50K total |
| Signup rate (anonymous → signed up) | 25% |
| Challenge completion rate (started → finished) | 70% |
| Share rate (completions → shares) | 15% |
| Schools active (10+ students) | 100 |
| Tutoring trials from RML | 50 |

### 60 Days Post-Launch

| Metric | Target |
|--------|--------|
| MAU | 40K |
| 7-day return rate | 35% |
| Challenge completion rate | 75% |
| Share rate | 20% |
| Schools active | 400 |
| Tutoring trials from RML | 200 |
| Trial-to-paid conversion (RML cohort) | 35% |

### 90 Days Post-Launch

| Metric | Target |
|--------|--------|
| MAU | 80K |
| Challenges in library | 150+ |
| Avg challenges / user / month | 4 |
| Schools active | 800 |
| Tutoring trials from RML | 500 |
| Revenue attributed to RML | $420K (500 trials x 35% conv x $2,400 LTV) |
| Organic traffic to /league/ pages | 20K visits/month from search |

## Risks and Mitigations

| Risk | Likelihood | Impact | Mitigation |
|------|-----------|--------|------------|
| Challenge quality inconsistent due to AI generation | Medium | High | Strict review checklist, every challenge playtested by a different person, quality over quantity |
| Low share rate — users complete but don't share | Medium | High | A/B test share card designs, make sharing feel rewarding (XP bonus), optimize card for platform (WhatsApp vs Instagram) |
| School adoption slower than projected | Medium | Medium | Start with Cuemath's existing school network (warm leads), offer teacher onboarding support, create showcase content |
| Conversion to tutoring negligible | Medium | High | Test multiple nudge surfaces and copy, ensure nudges feel natural not salesy, compare RML user quality vs. other channels |
| Technical issues at scale | Low | High | Load test before launch, CDN for static content, database indexing for leaderboard queries, monitoring + alerting |
| Competitive response (other platforms copy the model) | Low | Medium | Speed to market, brand moat (Cuemath's credibility), content quality, school network effects |
| Content runs out — users exhaust 100 challenges | Medium | Medium | Pipeline for continuous challenge creation (target 10-15/week post-launch), seasonal and trending topic challenges |
| Mobile experience subpar (desktop-first trade-off) | Medium | Medium | Ensure full functionality on mobile even if not optimized, prioritize mobile polish in post-launch sprints |

## Post-Launch Roadmap

### Month 2-3: Optimize
- Mobile experience optimization (dedicated mobile design pass)
- A/B testing results → implement winners
- Content expansion: 150 → 200 challenges
- Tutoring conversion funnel optimization
- School dashboard enhancements based on teacher feedback

### Month 3-6: Expand
- **New themes:** History, Art, Medicine, Environment, Sports analytics
- **Seasonal challenges:** Math of Halloween, Holiday shopping math, Olympics math, World Cup math
- **Challenge series:** Multi-challenge story arcs (e.g., "Build a City" — 5 connected challenges)
- **Regional content:** Market-specific challenges (US, India, Southeast Asia, Middle East)
- **Native mobile app** evaluation (if mobile traffic exceeds 40%)

### Month 6-12: Community
- **User-submitted challenges:** Allow teachers/students to propose challenge ideas
- **Live challenge events:** Time-limited challenges with real-time leaderboards (monthly)
- **School partnerships:** Co-branded challenges with schools, districts, education orgs
- **Math influencer collaborations:** Challenges co-created with math YouTubers / educators
- **API for schools:** Allow schools to embed RML challenges in their LMS
- **Cuemath student integration:** RML challenges as supplementary content for paid students

### Year 2 Vision
- RML as the front door to Cuemath — majority of new tutoring leads originate from RML
- 1M+ MAU with self-sustaining viral growth
- 500+ challenges across 15+ themes
- Global school leaderboard as a recognized institution
- RML brand becomes synonymous with "real-world math" in search and AI engines
