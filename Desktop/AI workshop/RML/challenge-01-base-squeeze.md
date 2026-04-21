---
type: challenge
series: The Volume Con
challenge: 1 of 3
title: The Base Squeeze
topic: Cuboid volume — how two small base cuts compound into a large loss
date: 2026-04-21
status: content locked
---

# Challenge 1 — The Base Squeeze

## Overview

| | |
|---|---|
| **Series** | The Volume Con |
| **Position** | Challenge 1 of 3 |
| **Core math** | V = L × W × H. Each dimension is linear alone. Two base dimensions cut together → compound loss. |
| **Real-world frame** | A viral WhatsApp complaint about ChocoBar — same price, quietly smaller bar |
| **Duration** | 12–18 minutes |
| **Level** | 3 (Grade 5) |
| **Mascot** | Pip |

---

## The Five

| | |
|---|---|
| **Hook** | A WhatsApp photo forwarded 200 times — "did ChocoBar get smaller or am I going crazy?" Company says nothing. |
| **Skill** | V = L × W × H. Each dimension contributes linearly alone, but cutting two base dimensions at once creates a compound loss. |
| **What the kid does** | Spot the base shrinkage visually. Predict the volume loss. Explore linearity. Run the simulation. Explain the company's logic. Apply to a new product. |
| **Aha** | Two 8% base cuts = 15.4% volume loss — because cuts multiply, not add. Same number, same mechanism as the cylinder in Challenge 2. |
| **Tool unlocked** | The Base Squeeze |

---

## Core Numbers

| | Length | Width | Height | Volume |
|---|---|---|---|---|
| **Original bar** | 20 cm | 10 cm | 2 cm | 400 cm³ |
| **New bar** | 18.4 cm | 9.2 cm | 2 cm | 338.6 cm³ |
| **Change** | −8% | −8% | 0% | −15.4% |

**Why these numbers:** The 15.4% loss from two 8% base cuts mirrors the 15.4% loss from an 8% radius cut in Challenge 2 (cylinder). Same mechanism. Same number. The connection lands when kids reach Challenge 2.

---

## Section-by-Section

---

### Section 1 — The Assignment

**Goal:** Hook the kid into the investigation. Establish that something changed with no company confirmation — just a feeling going viral.

---

**VISUAL — WhatsApp card**
A styled message bubble showing a forwarded photo.
- Two ChocoBar images side by side: old packaging vs new packaging
- Caption beneath: *"guys did ChocoBar change their bar or am I going crazy 😭"*
- Small detail: Forwarded 200 times

**PIP SAYS**
> "Companies don't have to announce a change. They just do it. No asterisk. No press release. Just a new design quietly on the shelves — and a growing number of people who feel like something's off.
> Your job: find out if the feeling is real."

**BUTTON**
→ Start investigating

---

### Section 2 — First Look

**Goal:** Kid spots that the base shrank — visually, before any numbers. This should feel like a genuine discovery, not something they're told.

---

**PIP SAYS**
> "Two bars. Same price. Same red. Take a look."

**VISUAL — SVG, top-down view**
Both bars shown from above — the view you actually get when you unwrap a chocolate bar.
From this angle, height is invisible. Length and width are fully visible.
The new bar looks subtly smaller but it's not immediately obvious — the difference is real but not dramatic.

**INTERACTION — Compare button**
A single "Compare" button below the visual.
On tap: the old bar's outline (dashed ghost) overlays on top of the new bar.
The new bar sits visibly smaller inside the ghost. The gap between the edges — the lost base area — is shaded in a soft coral colour.

**PIP SAYS** *(after Compare is tapped)*
> "See that gap? That's what changed. The base got smaller. Height is the same — you can't see height from above. But length and width? Right there."

**BUTTON**
→ Let's measure it

---

### Section 3 — The Measurements + Intuition

**Goal:** Reveal the actual numbers. Then immediately capture the kid's intuition — by how much did the chocolate actually reduce? Lock in the guess before any calculation happens.

---

**PIP SAYS**
> "Someone measured both bars. Here's what the ruler found."

**VISUAL — SVG with dimension arrows**
Two chocolate bars shown with full dimension annotations.
- Original bar: `L = 20 cm` (horizontal arrow, neutral colour), `W = 10 cm` (depth arrow, neutral colour), `H = 2 cm` (vertical arrow, neutral colour)
- New bar: `L = 18.4 cm` (coral arrow, showing reduction), `W = 9.2 cm` (coral arrow), `H = 2 cm` (same neutral colour — unchanged)

Both bars shown side by side. The unchanged height is visually obvious. The shorter L and W are annotated clearly.

**PIP SAYS**
> "Height: identical on both. Length and width: both smaller on the new bar. Both cut by 8%. No announcement. No asterisk on the wrapper. Just a new design."

**INTERACTION — Prediction cards**
> "Your chocolate shrank. Before you calculate anything — how much do you think is gone?"

| Card | Label |
|---|---|
| 📉 About 8% | One cut, one loss |
| 📉📉 About 16% | Two cuts, add them up |
| ❓ Something else | Neither of these |

Kid locks in their guess. No answer revealed yet — the guess is saved and returned to in Section 5.

---

### Section 4 — One Cut at a Time

**Goal:** Build the intuition that each dimension behaves linearly in isolation. This is essential groundwork — the surprise in Section 5 only lands if the kid first believes the cuts should add.

---

**PIP SAYS**
> "Before we look at what ChocoBar actually did — understand what each dimension does on its own. Move the slider."

**VISUAL — SVG**
Single chocolate bar. Ghost outline shows original size.
Volume stat pill below: `Volume remaining: 100%`
Dimension label updates live on the bar.

**INTERACTION — Slider: height**
Label: *Decrease height by*
Range: 0–30%
- Bar shrinks vertically as slider moves
- Ghost outline stays fixed — shows original height
- Stat pill updates live: e.g. `Volume remaining: 90%` at 10% cut
- Dimension label on bar updates: `H = 1.8 cm`

**CALLOUT** *(appears after slider is moved)*
> Cut height by 10% → volume drops by exactly 10%. One direction. One honest loss.

**INTERACTION — Slider swaps to: length**
Same bar, same ghost. Now slider controls length instead.
- Bar shrinks horizontally
- Stat pill updates the same way

**CALLOUT** *(updates)*
> Same result. Cut length 10% → lose 10%. Each dimension on its own is completely predictable.

**PIP SAYS** *(after both sliders explored)*
> "Simple, right? Change one dimension, lose that exact percentage. No tricks — yet."

**BUTTON**
→ Now watch what ChocoBar actually did

---

### Section 5 — The Simulation (The Aha)

**Goal:** The core moment. Kid runs the simulation with both base dimensions, sees the compound loss visually, and discovers that the answer is neither of their two obvious guesses. The Section 3 prediction is resolved here.

---

**PIP SAYS**
> "ChocoBar cut both length AND width by 8%. Not one — both. Set both sliders and see what happens."

**VISUAL — SVG, top-down grid view**
The bar's top face shown as a grid — like graph paper squares filling the base area.
Original bar's outline shown as ghost.
As sliders move, the grid shrinks in both dimensions simultaneously.
The squares that fall outside the new bar's area — the lost chocolate — are highlighted in coral.

**INTERACTION — Two sliders**

| Slider | Range | What updates |
|---|---|---|
| Decrease length by | 0–30% | Bar shrinks horizontally, `L = X cm` label updates, lost columns highlighted coral |
| Decrease width by | 0–30% | Bar shrinks in depth, `W = X cm` label updates, lost rows highlighted coral |

**STAT PILLS** *(below the grid, update live)*

| Pill | Example at 8% each |
|---|---|
| L | 18.4 cm |
| W | 9.2 cm |
| Volume remaining | 84.6% |
| Volume lost | 15.4% |

**CALLOUT** *(appears when both sliders reach 8%)*
> Length −8%, Width −8% → Volume lost: **15.4%**
> Not 8% — you cut two directions, not one.
> Not 16% — the second cut is 8% of a bar that's already 8% smaller. The cuts multiply, not add.

**PREDICTION RESOLUTION** *(appears below callout)*
> "Earlier you guessed: [their answer from Section 3]"
> The real answer: 15.4% gone.

If they guessed "Something else" → *"You sensed it. Neither 8% nor 16% — the answer sits between them because the cuts multiply."*
If they guessed 8% → *"A fair guess — but that would only be true if one dimension changed. Both changed."*
If they guessed 16% → *"Close instinct — two cuts, so double felt right. But the second cut is 8% of a smaller bar. The maths gives 15.4%, not 16%."*

**BUTTON**
→ But why the base?

---

### Section 6 — Why the Base?

**Goal:** Understand the company's logic. Height is tactile and instantly noticeable. Base dimensions are invisible without a ruler. This is what makes the trick work in real life.

---

**PIP SAYS**
> "ChocoBar could have made the bar 15% thinner. Same volume loss. Why didn't they?"

**INTERACTION — MCQ**

| Option | Text |
|---|---|
| A | Thinner chocolate breaks more easily during shipping |
| B ✓ | Height is what your hand feels immediately — thinner is noticed in seconds |
| C | The mold for the base is cheaper to change |
| D | Regulations require height to stay constant |

**FEEDBACK — correct (B)**
> Pick up any object. Your hand registers thickness before you even look at it — within a second of picking it up.
> But does anyone measure the length of their chocolate bar before eating it? That needs a ruler, a memory of the old size, and the effort to compare.
> ChocoBar is counting on no one doing that. Shrink the base — both dimensions, a little each — and the loss is real but invisible.

**FEEDBACK — wrong**
> Think about the moment you pick something up. What do your fingers notice first — how thick it is, or how long it is?

---

### Section 6b — Practice Question

**Goal:** Apply the skill to a new product. Confirm the kid can generalise, not just recall. Appears immediately below the correct answer feedback — no new section, no navigation.

---

**PRACTICE LABEL**
🏋️ Practice Question

**QUESTION**
> CrunchCo just quietly redesigned their cracker box. Height: unchanged. Length: cut by 6%. Width: cut by 6%.
> Your friend says: "they only cut 6% of the volume." Are they right?

**INTERACTION — MCQ**

| Option | Text |
|---|---|
| A | Yes — a 6% cut on both dimensions means 6% less overall |
| B | No — it's about 12% less (6 + 6) |
| C ✓ | No — it's about 11.6% less (0.94 × 0.94 = 0.8836) |

**FEEDBACK — correct (C)**
> Your friend added the cuts. But they multiply.
> 0.94 × 0.94 = 0.8836 — so 11.6% of the volume is gone. Not 12%. And definitely not 6%.
> Different box, different numbers. Same trick.

**FEEDBACK — wrong**
> Remember what happened with ChocoBar. When two base dimensions both shrink, the cuts don't add — they multiply. What is 0.94 × 0.94?

**BUTTON** *(appears after practice question is answered correctly)*
→ Name the trick

---

### Section 7 — Tool Unlock + Bridge

**Goal:** Name the mechanism. Give the kid the tool. Bridge cleanly to Challenge 2 by showing that the same mechanism applies to a circular base — and produces the same number.

---

**PIP SAYS**
> "Two directions. Both in the base. Both invisible without a ruler. Combined: a 15.4% loss from two cuts that each look like 8%."

**VISUAL — Tool unlock card**

```
┌─────────────────────────────────────────────┐
│  NEW TOOL UNLOCKED                          │
│                                             │
│  📐  The Base Squeeze                       │
│                                             │
│  When a company shrinks two base            │
│  dimensions instead of one, the cuts        │
│  multiply — not add. Two small cuts,        │
│  one surprisingly large loss.               │
│                                             │
│  And the base is always the hiding spot —   │
│  because nobody measures the length of      │
│  their chocolate bar before eating it.      │
└─────────────────────────────────────────────┘
```

**BRIDGE TEXT** *(below the tool card)*
> "Now here's what makes Challenge 2 different.
> ChocoBar has a rectangular base. You can shrink length and width separately — two distinct moves.
> What if the base is a circle? There's no length or width to shrink separately. Just a radius.
> Shrink the radius and you shrink the circle in every direction at once — both dimensions of the base in one move.
> Same trick. Rounder shape. And the volume loss from an 8% radius cut?
> Exactly 15.4%. For exactly the same reason."

**BUTTON**
→ Challenge 2: The Crisps Can

---

## Interactions Summary

| Section | Interaction type | Purpose |
|---|---|---|
| 1 | None — read + button | Set up the investigation |
| 2 | Compare button → ghost overlay | Kid discovers the base shrank visually |
| 3 | Prediction cards (3 options) | Capture intuition before calculation |
| 4 | Two sliders sequentially (height, then length) | Build the "each dimension is linear" intuition |
| 5 | Two simultaneous sliders + live grid simulation | Discover the compound effect; resolve the Section 3 guess |
| 6 | MCQ | Understand why companies target the base |
| 6b | MCQ (practice) | Apply the skill to a new product |
| 7 | None — tool unlock + bridge | Name the mechanism, set up Challenge 2 |

---

## Prediction Resolution Logic (Section 5)

| Kid's Section 3 guess | Resolution message |
|---|---|
| About 8% | "A fair guess — but that's only true if one dimension changes. Both changed here." |
| About 16% | "Close instinct — two cuts felt like double. But the second cut is 8% of a smaller bar. The maths gives 15.4%, not 16%." |
| Something else | "You sensed it. Neither 8% nor 16% — the answer sits between them because the cuts multiply." |

---

## Visual Specifications

| Section | Visual type | Key elements |
|---|---|---|
| 1 | Styled card | WhatsApp message bubble, two bar photos, forward count |
| 2 | SVG — top-down view | Two bars from above, ghost overlay on Compare tap, coral shading on lost area |
| 3 | SVG — with dimension arrows | Neutral arrows for unchanged dims, coral arrows for changed dims |
| 4 | SVG — single bar with ghost | Bar updates live with slider, ghost stays fixed |
| 5 | SVG — top-down grid | Grid squares fill the base area, lost squares highlight coral as sliders move |
| 6 | None | Just Pip + MCQ |
| 6b | None | Just practice question block |
| 7 | Tool unlock card | Navy card, tool name, icon, description, bridge text |

---

## Bridge to Challenge 2

Challenge 2 (The Crisps Can) opens with the same 8% cut — but now on a cylinder's radius. The r² in V = πr²h exists precisely because the radius controls both dimensions of the circular base simultaneously. The Base Squeeze tool from Challenge 1 is the conceptual foundation that makes this land without the formula feeling arbitrary.

---

## Scope Boundary

This challenge deliberately does NOT cover:
- Cone volume (Challenge 3)
- The r² formula (Challenge 2)
- Any formula beyond V = L × W × H
- Percentage arithmetic beyond simple multiplication
