---
type: challenge
series: The Volume Con
challenge: 3 of 3
title: The Hollow Illusion
topic: Cone volume — why fill height and fill volume are completely different things
date: 2026-04-21
status: content locked
---

# Challenge 3 — The Hollow Illusion

## Overview

| | |
|---|---|
| **Series** | The Volume Con |
| **Position** | Challenge 3 of 3 |
| **Core math** | At fill height h in a cone of total height H: radius at that level = (h/H) × R (similar triangles). Area at that level = π((h/H)R)² = (h/H)² × πR². Volume filled = (h/H)³ × total volume. |
| **Real-world frame** | A restaurant serves a drink in a conical glass filled to 80% of its height. How full is it really? |
| **Duration** | 15–20 minutes |
| **Level** | 5 (Grade 7) |
| **Mascot** | Pip |

---

## The Five

| | |
|---|---|
| **Hook** | A conical glass filled to 80% of its height. Looks almost full. How much of the glass is actually filled with liquid? |
| **Skill** | Similar triangles → radius grows linearly with height. But area = πr² → area grows as height². Volume = (h/H)³ × total — grows as height cubed. |
| **What the kid does** | Guess the fill fraction. Explore why the shape matters. Discover that radius scales linearly. Discover that area scales as the square. Run the simulation. Calculate the real answer. Apply to a new shape. |
| **Aha** | At 80% height the glass is only 51.2% full. The top 20% of height holds 48.8% of the volume — a gap that looks small but hides nearly half the drink. |
| **Tool unlocked** | The Hollow Illusion |

---

## Core Numbers

| Fill height | Radius at that level | Circle area at that level | Volume filled |
|---|---|---|---|
| 25% of H | 25% of R | 6.25% of full area | 1.56% of total |
| 50% of H | 50% of R | 25% of full area | 12.5% of total |
| 75% of H | 75% of R | 56.25% of full area | 42.2% of total |
| 80% of H | 80% of R | 64% of full area | 51.2% of total |
| 90% of H | 90% of R | 81% of full area | 72.9% of total |
| 100% of H | 100% of R | 100% of full area | 100% of total |

**The challenge uses 80% fill height throughout** — producing the most striking result (barely over half full) while being a realistic fill level for a drink.

---

## Section-by-Section

---

### Section 1 — The Setup

**Goal:** Hook the kid with a concrete, visual scenario. No math yet — just the situation and the question.

---

**VISUAL — Restaurant scene card**
A styled card showing a conical cocktail glass — the elegant, V-shaped kind. The liquid is clearly visible, filled close to the rim. The glass looks generous and almost full. No numbers shown yet.

**PIP SAYS**
> "A restaurant serves their signature drink in this glass. It's filled close to the rim — looks almost full.
> Here's the question you're going to answer today: how full is it actually?"

**BUTTON**
→ Let's find out

---

### Section 2 — Take a Guess

**Goal:** Capture the kid's intuition before any math. The guess is saved and returned to in Section 7 — the payoff. Most kids will guess 70–80%, making the real answer (51.2%) genuinely surprising.

---

**VISUAL — Conical glass with fill marker**
The conical glass shown clearly from the side.
A horizontal dashed line marks the liquid level.
A label on the side: **fill height = 80% of the glass**
The liquid below the line is filled in. The gap above is empty.
The glass looks nearly full — this is intentional.

**PIP SAYS**
> "The liquid reaches 80% of the glass's height. That gap at the top looks small.
> Before any calculation — what fraction of the glass do you think is filled with liquid?"

**INTERACTION — Prediction cards**

| Card | Label |
|---|---|
| 🥤 About 80% | The height tells you the volume |
| 🥤 About 60–65% | A bit less than the height |
| 🥤 Less than 50% | Much less than it looks |

Kid locks in their guess. No answer revealed yet. The guess is stored.

---

### Section 3 — Why Does the Shape Matter?

**Goal:** Build the intuition that a cone's cross-section changes at every height — unlike a cylinder where every level is identical. This is the key difference that makes cone volume behave non-linearly.

---

**PIP SAYS**
> "Before we calculate — just look at the glass. Something about this shape is different from anything we've seen before."

**VISUAL — Conical glass from the side, interactive**
The glass shown as a real conical shape (not a triangle — a glass outline with liquid inside).
Two tap targets on the glass:

**INTERACTION — Explore buttons (tap on the glass at two heights)**

| Tap location | What appears |
|---|---|
| Near the bottom of the glass | A thin horizontal circle appears across the glass at that level. Label: "At the bottom — the glass is narrow here. This circle is small." |
| Near the top of the glass | A wide horizontal circle appears. Label: "At the top — the glass is wide here. This circle is much larger." |

**PIP SAYS** *(after both are tapped)*
> "Every level of this glass is a different-sized circle. At the bottom: a tiny circle. At the top: a big circle. The width keeps growing as you go up.
> That's what makes this shape different. And that's what makes the volume surprising."

**BUTTON**
→ How much does the width grow?

---

### Section 4 — The Radius Grows With Height

**Goal:** Introduce similar triangles as the tool that lets you calculate the radius at any fill level. Make the proportional relationship concrete and interactive before introducing any algebra.

---

**PIP SAYS**
> "Look at the glass from the side. The walls are straight lines — not curved. That straight wall is the key."

**VISUAL — Glass side view with triangle overlay**
The glass outline shown from the side — a triangle shape with the tip at the bottom, widening upward.
The full triangle: height H, base radius R at the top.
A second, smaller triangle drawn inside it up to a fill height h — same shape, just smaller.
Both triangles have the same angles. They are similar triangles.

**PIP SAYS**
> "These two triangles have the same shape — just different sizes. That's what 'similar triangles' means.
> Because they're similar: the ratio of sides is the same.
> r / R = h / H
> So at any fill height: **r = (h/H) × R**"

**INTERACTION — Height picker**
Three buttons: 25% / 50% / 75%
Kid taps each. For each:
- The fill level is marked on the glass
- The radius at that level is shown as a horizontal arrow
- The calculation appears: e.g. "At 50% height: r = 0.5 × R = half the full radius"

| Height tapped | Radius shown | Calculation displayed |
|---|---|---|
| 25% | r = R/4 | "At 25% height: r = 0.25 × R" |
| 50% | r = R/2 | "At 50% height: r = 0.50 × R" |
| 75% | r = 3R/4 | "At 75% height: r = 0.75 × R" |

**CALLOUT** *(appears after all three are tapped)*
> The radius grows evenly with height — it's a straight-line relationship.
> Go up 10% more height → radius grows 10% more. Predictable, linear.

*Feel: I can find the radius at any fill level. It scales simply.*

---

### Section 5 — But the Circle Grows Faster

**Goal:** The key conceptual leap. Radius grows linearly — but area = πr², so area grows as the square of height. This is the same insight as Challenge 2 (radius is squared), now applied to a new shape. The circle comparison makes the non-linearity visually striking.

---

**PIP SAYS**
> "The radius at 50% height is 50% of the full radius. So the circle at 50% height must be 50% of the full circle — right?"

**INTERACTION — Guess**
Two buttons: ✅ Yes, 50% / ❌ No, something else
Both lead forward (this is a diagnostic, not scored).

**VISUAL — Two circles side by side**
Circle A: the full circle at 100% height (radius = R). Labelled "Top of glass".
Circle B: the circle at 50% height (radius = R/2). Labelled "Halfway up".

Circle B sits visibly inside Circle A — it's dramatically smaller. Not half the size. Much smaller.

**PIP SAYS**
> "The radius halved — from R to R/2. But the area didn't halve.
> Area = πr². At 50% height: area = π(R/2)² = πR²/4.
> **Just 25% of the full circle** — not 50%."

**VISUAL — Area comparison with numbers**

| Height | Radius | Circle area |
|---|---|---|
| 100% | R | 100% of full circle |
| 75% | 3R/4 | 56.25% of full circle |
| 50% | R/2 | 25% of full circle |
| 25% | R/4 | 6.25% of full circle |

**CALLOUT**
> This is the same reason from Challenge 2: radius is squared in the area formula.
> When radius halves, area quarters. When radius is 75%, area is only 56%.
> The circles near the bottom are tiny. The circles near the top are huge.
> Volume is piling up at the top — not evenly distributed through the glass.

**BUTTON**
→ See it happen live

---

### Section 6 — The Fill Simulation

**Goal:** Let the kid experience the non-linear fill directly. The simulation makes the (h/H)³ relationship visceral — seeing how slowly volume accumulates at the bottom and how quickly it surges at the top.

---

**PIP SAYS**
> "Now fill the glass yourself. Watch what happens to the volume."

**VISUAL — Conical glass, fill slider**
The glass shown from the side. Liquid fills from the bottom as the slider moves.
The liquid colour fills in visibly. Ghost markers show the full glass outline.

**INTERACTION — Fill slider**
Range: 0–100% height
Live updates:
- Liquid fills the glass visually up to slider level
- Horizontal dashed line marks current fill height
- Stat pills update:

**STAT PILLS**

| Pill | Example at 80% |
|---|---|
| Fill height | 80% |
| Volume filled | 51.2% |

**CALLOUT — appears at specific moments as kid moves slider**

| Slider position | Callout text |
|---|---|
| Reaches 50% | "Halfway up the glass — but only 12.5% of the volume. The bottom half of the glass is mostly narrow circles." |
| Reaches 80% | "80% of the height — but only 51.2% of the volume. You need the top 20% for the other half." |
| Reaches 90% | "90% of the height — finally 72.9% of the volume. Almost all the volume lives in the top portion." |
| Reaches 100% | "100% — the full glass. The last 10% of height contained 27.1% of the volume." |

**PIP SAYS** *(after slider is explored)*
> "Radius grows linearly. Area grows as radius squared. Volume grows as height cubed.
> Volume filled = (h/H)³ × total volume.
> That's why the glass fills so slowly at the bottom and so quickly at the top."

---

### Section 7 — Back to the Restaurant Glass

**Goal:** Return to the original question from Section 2. Apply the formula to the specific glass. Reveal and resolve the prediction. The gap that looked small turns out to hold nearly half the volume.

---

**PIP SAYS**
> "Back to that restaurant glass. Filled to 80% of its height."

**VISUAL — The original glass from Section 2**
The same conical glass, filled to 80% height. Now with the formula overlaid.

**CALCULATION — step by step reveal**

```
Fill height  = 80% = 0.8
Volume filled = (0.8)³ × total
             = 0.512 × total
             = 51.2% of the glass
```

**VISUAL — Split view**
Left: the glass with liquid filled to 80% height.
Right: the same glass with the 51.2% fill marked differently — showing that the top 20% of height holds 48.8% of the total volume. That "small gap" at the rim is highlighted.

**CALLOUT**
> The gap at the top looks small. But it holds **48.8% of the glass's total volume.**
> Half the drink lives in the top 20% of height.

**PREDICTION RESOLUTION**

| Kid's Section 2 guess | Resolution message |
|---|---|
| About 80% | "The height was 80% — but volume doesn't follow height directly. Because the radius is squared, volume follows height cubed. 0.8³ = 0.512." |
| About 60–65% | "Good instinct that it would be less — but it's even less than that. The squaring of the radius pulls the number down further than most people expect." |
| Less than 50% | "You sensed it — the shape was hiding more than it looked. Exactly right: 51.2%, just over half." |

---

### Section 7b — Practice Question

**Goal:** Apply the (h/H)³ formula to a new scenario. Confirm the kid can generalise beyond the restaurant glass.

---

**PRACTICE LABEL**
🏋️ Practice Question

**QUESTION**
> An ice cream cone is filled to 75% of its height with ice cream. What fraction of the cone's capacity is actually filled?

**INTERACTION — MCQ**

| Option | |
|---|---|
| A | About 75% — same as the height fraction |
| B | About 56% — radius is squared so a bit less |
| C ✓ | About 42% — (0.75)³ = 0.422 |

**FEEDBACK — correct (C)**
> 0.75³ = 0.421875 — just over 42%.
> A cone that looks three-quarters full is barely two-fifths full.
> The radius-squared effect from Challenge 2 is still here — just applied twice now, because volume grows as height cubed.

**FEEDBACK — wrong**
> Remember: volume = (h/H)³ × total. At 75% height, that's 0.75³. Try calculating that — it's smaller than you expect.

**BUTTON** *(appears after correct answer)*
→ Collect your tool

---

### Section 8 — Tool Unlock + Series Close

**Goal:** Name the mechanism. Unlock the final tool. Close the series by connecting all three challenges — one pattern, three shapes.

---

**PIP SAYS**
> "The glass looked 80% full. It was 51.2% full. The gap that looked like a sliver held nearly half the drink. That's not a flaw in your perception — it's geometry."

**VISUAL — Tool unlock card**

```
┌─────────────────────────────────────────────┐
│  NEW TOOL UNLOCKED                          │
│                                             │
│  🔺  The Hollow Illusion                    │
│                                             │
│  In a cone, volume grows as the cube        │
│  of the height fraction.                    │
│                                             │
│  Fill to 80% of the height →               │
│  only 51.2% of the volume.                  │
│                                             │
│  The top of the cone holds a               │
│  disproportionate share of the volume —     │
│  which means what looks almost full         │
│  can be mathematically half empty.          │
└─────────────────────────────────────────────┘
```

**SERIES CLOSE — Three tools, one pattern**

```
┌─────────────────────────────────────────────────────────────┐
│  THE VOLUME CON — COMPLETE                                   │
│                                                              │
│  📐 The Base Squeeze                                         │
│     Two base dimensions cut together → cuts multiply,        │
│     not add. The base is where the loss hides.              │
│                                                              │
│  🔵 The Hidden Lever                                         │
│     Radius is squared in the volume formula.                 │
│     A small radius cut hits harder than it looks.           │
│                                                              │
│  🔺 The Hollow Illusion                                      │
│     Volume grows as height cubed in a cone.                  │
│     A nearly full glass can be mathematically half empty.   │
│                                                              │
│  One pattern across all three:                               │
│  The volume is always hiding in a dimension you             │
│  weren't watching.                                          │
└─────────────────────────────────────────────────────────────┘
```

---

## Interactions Summary

| Section | Interaction type | Purpose |
|---|---|---|
| 1 | None — read + button | Set the scene |
| 2 | Prediction cards (3 options) | Capture intuition before calculation |
| 3 | Explore taps (2 points on glass) | Discover that cross-sections change with height |
| 4 | Height picker (3 buttons) | Discover the linear radius-height relationship |
| 5 | Guess button + visual reveal | Discover that area grows as radius squared |
| 6 | Fill slider + live stat pills | Experience the cubic volume relationship directly |
| 7 | Calculation reveal + prediction resolution | Apply formula, resolve Section 2 guess |
| 7b | MCQ (practice) | Apply to a new shape |
| 8 | None — tool unlock + series close | Name the mechanism, close the series |

---

## Prediction Resolution Logic (Section 7)

| Kid's Section 2 guess | Resolution message |
|---|---|
| About 80% | "The height was 80% — but volume doesn't follow height directly. Radius is squared, so volume follows height cubed. 0.8³ = 0.512." |
| About 60–65% | "Good instinct that it's less — but the squaring of the radius pulls the number down further than expected. It's 51.2%." |
| Less than 50% | "You sensed it. The shape hides more than it shows. Exactly right — 51.2%, just barely over half." |

---

## Visual Specifications

| Section | Visual type | Key elements |
|---|---|---|
| 1 | Styled card | Elegant conical glass, liquid near rim, no numbers |
| 2 | SVG — conical glass with fill marker | 80% fill line marked, liquid filled below, gap above clearly visible |
| 3 | SVG — interactive glass | Two tap targets at different heights, circle cross-sections appear on tap |
| 4 | SVG — side view with triangle overlay | Full triangle + smaller similar triangle, radius arrows at 25/50/75% |
| 5 | SVG — two circles side by side | Full circle vs circle at 50% height, area comparison table |
| 6 | SVG — fill slider animation | Liquid fills from bottom, stat pills update live, callouts at key heights |
| 7 | SVG — split view | Left: 80% fill height. Right: 51.2% volume marked, top gap highlighted |
| 7b | None | Practice question block |
| 8 | Two cards | Tool unlock card + series complete card |

---

## The Math Chain (for reference)

**Step 1 — Similar triangles give the radius at any fill height:**
r / R = h / H → r = (h/H) × R

**Step 2 — Area at any fill height:**
Area = πr² = π × ((h/H) × R)² = (h/H)² × πR²

**Step 3 — Volume up to fill height h:**
Each thin slice at height y has area = (y/H)² × πR²
Adding all slices from 0 to h: Volume = (h/H)³ × (1/3)πR²H = (h/H)³ × V_total

The kid is not shown the integration. They see the (h/H)³ result emerge from the simulation in Section 6, and understand it as: radius grows linearly (Section 4), area grows as the square (Section 5), volume grows as the cube (Section 6).

---

## Scope Boundary

This challenge deliberately does NOT cover:
- The (1/3) factor in the cone volume formula (addressed in the full cone volume formula only if taught separately)
- Integration or formal calculus
- Comparison between cone and cylinder volumes
- Any ml or quantity claims about the restaurant
