---
type: design
topic: Real Math League — Experience Design
date: 2026-04-07
status: draft
version: 1
---

# Real Math League — Experience Design

## Information Architecture

```
cuemath.com/league/
├── /                              Homepage — featured challenges, themes, leaderboard preview
├── /challenges/                   Browse all challenges (filterable)
├── /challenges/{slug}/            Challenge detail page
├── /challenges/{slug}/play/       In-challenge experience (step-by-step)
├── /challenges/{slug}/complete/   Completion screen + share card
├── /leaderboard/                  Leaderboard hub (school / city / grade tabs)
├── /leaderboard/schools/          School rankings
├── /leaderboard/cities/           City rankings
├── /leaderboard/grades/           Grade-level rankings
├── /profile/                      User profile (signed-in only)
├── /profile/badges/               Badge collection
├── /teachers/                     Teacher landing page + dashboard
├── /teachers/dashboard/           Class management + progress view
├── /about/                        What is Real Math League
└── /signup/                       Signup / login page
```

All pages live under `cuemath.com/league/` — fully integrated into the main domain, not a subdomain. This maximizes SEO value and brand cohesion.

## Homepage (`/league/`)

The homepage is the storefront. It must communicate instantly: this is not homework, this is exploration.

### Layout (top to bottom)

**1. Hero Section**
- Full-width dark background with vibrant accent illustration
- Rotating featured challenge with hook question: *"Why are manholes round?"*
- Large, confident headline: **"Real math. Real world. Real fun."**
- CTA: "Start Exploring" (no signup language)
- Subtle animation — numbers, shapes, patterns floating in background

**2. Theme Carousel**
- Horizontal scroll of theme cards: Nature, Sports, Space, Food, Cities, Music, Money, Architecture, Games, Technology
- Each theme has a distinctive icon and color
- Tapping a theme filters to challenges in that category

**3. Trending Challenges Grid**
- 6-8 challenge cards in a responsive grid
- Sorted by popularity (completion count) this week
- Each card: illustration, title, theme tag, level badge, time estimate, completion count
- "View all challenges" link at bottom

**4. How It Works**
- Three steps, illustrated:
  1. **Pick a challenge** — Browse real-world math explorations
  2. **Explore and solve** — Work through multi-step investigations
  3. **Share your discovery** — Earn XP, climb leaderboards, challenge friends
- Clean, minimal section. No jargon.

**5. Leaderboard Preview**
- Top 5 schools this week with XP totals
- "Find your school" search bar
- "View full leaderboard" link

**6. Footer CTA**
- "No signup needed. Just pick a challenge and go."
- Large "Browse Challenges" button

## Challenge Browsing (`/challenges/`)

### Filters (sticky top bar)
- **Theme:** All / Nature / Sports / Space / Food / Cities / Music / Money / Architecture / Games / Technology
- **Level:** All / Level 1-7 (maps to grades 3-10)
- **Duration:** All / Under 10 min / 10-20 min / 20-30 min
- **Sort:** Trending / Newest / Most Completed / Highest Rated

### Challenge Card Design
Each card in the grid contains:
- **Illustration** — Custom visual for the challenge (top 60% of card)
- **Title** — Bold, intriguing (e.g., "The Pizza Problem")
- **Hook** — One-line teaser (e.g., "Is the biggest pizza always the best deal?")
- **Theme tag** — Color-coded pill (e.g., "Food")
- **Level badge** — Small indicator (e.g., "Level 3")
- **Time estimate** — Clock icon + "15 min"
- **Completion count** — People icon + "2.4K completed"

Cards have a subtle hover animation (slight lift + shadow). Clicking goes to the challenge detail page.

### Grid Layout
- Desktop: 4 columns
- Tablet: 3 columns
- Mobile: 2 columns (stacked)
- Infinite scroll with lazy loading (no pagination)

## Challenge Detail Page (`/challenges/{slug}/`)

The detail page is the "movie poster" for each challenge. It must build anticipation.

### Layout

**1. Hero Section (full-width)**
- Large challenge illustration as background (with dark gradient overlay)
- Challenge title (large, white, bold)
- Hook question in italic below title
- Theme tag + Level badge + Duration + Completion count (horizontal row)

**2. Accept Challenge CTA**
- Prominent button: "Accept Challenge"
- Below button: "No signup needed. Start right away."
- If signed in: "Accept Challenge" (with XP reward shown)

**3. What You'll Explore**
- 3-4 bullet points teasing what the challenge covers
- Does not spoil the answer / insight
- Builds curiosity

**4. Difficulty Meter**
- Visual bar showing difficulty (not intimidating — framed as "How deep does this go?")
- Labels: "Quick Dive" / "Steady Swim" / "Deep Exploration"

**5. Related Challenges**
- 3-4 cards of similar challenges (same theme or level)
- "More in [Theme]" header

**6. SEO Content Block**
- 100-200 words of context about the real-world topic (hidden behind "Learn more" toggle)
- Rich with keywords for search indexing

## In-Challenge Experience (`/challenges/{slug}/play/`)

This is the core product. Every design decision must serve two goals: delight and learning.

### Step-by-Step Flow

Each challenge is a linear sequence of 5-12 steps. The user progresses through them in order. No skipping.

**Step anatomy:**
```
┌─────────────────────────────────────────┐
│  Progress Bar (Step 3 of 8)             │
├─────────────────────────────────────────┤
│                                         │
│  [Visual Context]                       │
│  Rich illustration, diagram, photo,     │
│  or animation relevant to this step     │
│                                         │
├─────────────────────────────────────────┤
│                                         │
│  Narrative text — sets up the question  │
│  for this step. Conversational tone.    │
│  "Now imagine you're the architect..."  │
│                                         │
├─────────────────────────────────────────┤
│                                         │
│  [Input Area]                           │
│  MCQ / Numeric / Slider / Text / Audio  │
│                                         │
├─────────────────────────────────────────┤
│  [Submit / Next]                        │
└─────────────────────────────────────────┘
```

### Progress Bar
- Top of screen, always visible
- Shows current step out of total
- Filled segments for completed steps, current step highlighted, future steps dimmed
- Subtle animation on step completion

### Visual Context
- Every step has a visual element — no exceptions
- Types: custom illustration, annotated diagram, photo with overlay, simple animation, interactive widget
- Visuals are not decorative — they carry information and build context
- Responsive: full-width on mobile, constrained max-width on desktop

### Narrative Text
- Conversational, second-person ("You're standing at the base of the Eiffel Tower...")
- Short paragraphs (2-3 sentences max per block)
- Builds on previous steps — the story progresses
- Never lectures. Asks, provokes, invites

### Input Methods

| Type | Use Case | UX |
|------|----------|-----|
| **MCQ** | Conceptual understanding, estimation | 3-4 options, card-style (not radio buttons), immediate feedback |
| **Numeric** | Calculation, measurement | Large number input, keypad on mobile, unit label visible |
| **Slider** | Estimation, range exploration | Visual slider with real-time feedback on what the value means |
| **Text** | Open-ended reasoning, explanation | Multi-line text area, 2-3 sentence prompt, "Why do you think...?" |
| **Audio** | Verbal reasoning (younger kids) | Record button, 30-60 second limit, playback before submit |

### Feedback After Each Step
- **Correct (objective):** Green confirmation + brief explanation of why
- **Insightful (open-ended):** "Great thinking!" + model response shown for comparison
- **Incorrect:** No harsh "wrong" — instead, "Not quite. Here's a hint..." with one retry, then show the answer with explanation
- Feedback is always educational, never punitive

### No Timer by Default
- Timer is optional, off by default
- Can be enabled for competitive mode (leaderboard ranking considers speed as tiebreaker)
- If enabled, displayed subtly — not a pressure element

## Completion Screen (`/challenges/{slug}/complete/`)

The climax of the experience. This is where virality happens.

### Sequence (animated, 3-5 seconds)

1. **Celebration animation** — Confetti / particle burst / stars (theme-appropriate)
2. **Score reveal** — Large animated number, XP earned
3. **Key insight** — The "aha" moment: "Honeycombs are hexagons because hexagons tile with no gaps and use the least wax. Nature optimized before humans did."
4. **Score breakdown:**
   - Accuracy: X/Y correct
   - Reasoning quality: rating on open-ended responses
   - Exploration bonus: completed all steps

### Post-Score Actions

**Share Card** (prominent)
- Auto-generated branded card with:
  - Challenge illustration
  - Challenge name
  - User's score
  - Hook teaser ("I discovered why GPS needs 4 satellites. Can you?")
  - Cuemath RML branding
  - QR code linking to the challenge
- One-tap share: WhatsApp, Instagram Story, Copy Link, Download Image
- Card design variations (2-3 templates) tested for share rate

**Challenge a Friend**
- Generate a challenge link with user's score as the benchmark
- "I scored 850. Beat me?" — pre-filled share text
- Deep link opens the challenge directly

**Try Another**
- 2-3 recommended next challenges (same theme or next level)
- "Continue your streak" messaging if applicable

**Tutoring Nudge** (soft)
- Small card below main actions
- "Loved this? Explore 1:1 tutoring with Cuemath"
- Only after 2+ completed challenges
- Dismissible, non-intrusive

## Leaderboard Page (`/leaderboard/`)

### Tabs
- **Schools** — Default view. Schools ranked by total XP
- **Cities** — Cities ranked by aggregate student XP
- **Grades** — Top performers per grade level

### School Leaderboard
- Rank, school name, city, country, total XP, student count, top challenge
- Weekly and All-Time toggle
- Top 3 highlighted with gold/silver/bronze visual treatment
- "Find your school" search bar (prominent)
- If school not found: "Add your school" flow

### City Leaderboard
- Rank, city name, country, total XP, school count, student count
- Designed to drive city-level pride and competition

### Grade Leaderboard
- Filter by grade (3-10)
- Individual student rankings (display name only, privacy-safe)
- Top 10 with profile badges visible

## Profile Page (`/profile/`)

Signed-in users only. The personal dashboard.

### Layout

**1. Header**
- Display name, avatar (auto-generated from initials), level badge
- Total XP, current level, progress bar to next level
- Member since date, current streak

**2. Challenges Completed**
- Grid of completed challenge cards with scores
- Sortable by date, score, theme
- "Replay" option on each

**3. Theme Breakdown (Radar Chart)**
- Hexagonal radar chart showing performance across themes
- Axes: Nature, Sports, Space, Food, Cities, Music, Money, Architecture, Games, Technology
- Fills based on challenges completed and scores in each theme
- Visual indicator of strengths and exploration gaps

**4. Badges**
- Achievement badges earned:
  - "First Steps" — Complete 1 challenge
  - "Explorer" — Complete challenges in 3 different themes
  - "Deep Diver" — Score 900+ on any challenge
  - "Streak Master" — 7-day streak
  - "School Champion" — #1 in your school
  - "Century" — Complete 100 challenges
- Locked badges shown as silhouettes with hints

**5. Streak Calendar**
- GitHub-style contribution grid showing daily activity
- Current streak prominently displayed

## Design Principles

### Visual Language

**"Gaming feel, not school feel"**

- **Dark hero sections** — Deep navy / charcoal backgrounds for hero areas and the in-challenge experience. Creates focus and a premium, immersive feel.
- **Vibrant accents** — Electric blue, warm orange, bright green as accent colors. Every theme has a signature color.
- **Large, confident typography** — Headlines in a bold geometric sans-serif. Body text in a clean, readable sans-serif. Generous sizing.
- **Card-based layouts** — Everything is a card: challenges, leaderboard entries, badges, achievements. Cards have subtle depth (shadow + border-radius).
- **Micro-interactions** — Button hover effects, progress bar animations, score counter animations, card flip reveals. Every interaction has feedback.
- **Illustrations over photos** — Custom illustrated style for challenge visuals. Consistent, ownable, reproducible by AI. Flat with subtle gradients, not 3D.

### Tone

Every touchpoint reinforces: **math is cool, you are capable, this is fun.**

- Never use the word "test" or "exam"
- Never show a red "X" for wrong answers
- Celebrate effort, not just correctness
- Use "explore" and "discover" instead of "learn" and "study"
- Challenges have names, not numbers — personality matters

### Cardinal Rules (applied to design)

1. **Never intimidating** — No timers by default, no harsh failure states, difficulty framed positively, gentle retry mechanics
2. **Never boring** — Rich visuals on every step, varied input types, narrative progression, surprise moments in challenges
3. **Never traditional** — No worksheets, no textbook layouts, no classroom aesthetics, no clip art

## Accessibility

- WCAG 2.1 AA compliance as baseline
- All images have descriptive alt text
- Color is never the sole indicator of meaning (icons + labels accompany color coding)
- Keyboard navigation for all interactive elements
- Screen reader compatible challenge flow (step content read aloud)
- Audio input option benefits users with motor difficulties
- Text sizing respects browser/OS preferences
- Sufficient contrast ratios on all text (especially on dark backgrounds)

## Mobile Responsiveness

RML is **desktop-first** but must be fully functional on mobile.

### Desktop (primary)
- Full experience as designed above
- Challenge visuals at maximum fidelity
- Side-by-side layouts where applicable
- Hover interactions active

### Tablet
- Single-column challenge flow
- Theme carousel becomes horizontally scrollable
- Challenge grid: 3 columns → 2 columns
- Touch-friendly tap targets (minimum 44px)

### Mobile
- Single-column everything
- Challenge cards stack vertically (2-column grid)
- In-challenge: visual context above, input below (no side-by-side)
- Bottom-anchored "Submit" button for thumb reach
- Simplified leaderboard view (key data only)
- Share card optimized for mobile share sheet
- Audio recording works with device microphone
- No functionality removed — just reflowed for smaller screens
