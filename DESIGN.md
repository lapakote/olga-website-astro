<!-- SEED: re-run /impeccable document once there's code to capture the actual tokens and components. -->
---
name: Абрамова Ольга
description: Личный сайт социального и организационного психолога и антрополога — научная авторитетность в светлой, дерзкой подаче
colors:
  bg-quiet-fog: "#eeeeee"
  ink-deep-graphite: "#282828"
  accent-signal-orange: "#ff9737"
  neutral-cool-slate: "#d2dbda"
---

# Design System: Абрамова Ольга

## 1. Overview

**Creative North Star: "The Bright Observatory"**

A decisive IT-руководитель or conference organizer opens this site in the evening, deciding whether to bring Olga in. The system answers with daylight clarity, not theatrical darkness: a near-white, cool-toned surface (Pantone 2026 white, the shade the market's top players actually ship in 2026), deep graphite ink standing in for pure black, and exactly one accent — a decisive signal orange — that shows up only where a real action or insight lives. This is what "global strategist-visionary" looks like when it refuses the typical-coach cream palette on one side and the typical-tech-startup electric blue on the other.

The system explicitly rejects: cream/beige/sand "coach site" tones and handwritten script fonts; the stiff departmental-tile feel of a corporate university page; and the loud CTA buttons, countdown timers, and "transformation in 3 days" urgency copy of infobiznes/guru sites.

**Key Characteristics:**
- Bright, cool-neutral surface by default — light because clarity and scale read better than mood lighting, not because light is "safe"
- Deep graphite (not pure black) carries text and structure, avoiding both harsh AA contrast and washed-out gray
- Signal orange is rare and decisive: one CTA, one highlighted insight per screen, never decorative
- Cool slate-mist panels alternate with the fog background to create contrast blocks (machinescanthink.ai's dynamic without going dark)
- A single bold grotesque sans carries the whole system; richness comes from weight and scale jumps, not font-mixing
- Motion is choreographed: full-bleed video intro, scroll-driven reveals and transforms, not simple fades

## 2. Colors

A two-neutral, one-accent system: confident in daylight, decisive only where it needs to be.

### Primary
- **Signal Orange** (#ff9737): The one decisive accent — primary CTAs, the single highlighted phrase or data point per section, active states. Never ambient decoration.

### Neutral
- **Quiet Fog** (#eeeeee): Default page background. A true cool-toned light gray, not a warm cream — this is what keeps the site out of "typical expert site" territory.
- **Deep Graphite** (#282828): Primary ink for headlines and body text, plus structural dividers. Stands in for pure black without the harshness.
- **Cool Slate Mist** (#d2dbda): Secondary surface for alternating contrast blocks (full-bleed sections, footer, panel backgrounds) — the site's answer to machinescanthink.ai's block contrast without leaving the light register.

### Named Rules
**The Single Spark Rule.** Signal Orange appears once per screen: the one action or insight that matters most. If it shows up twice in the same viewport, something is wrong.

**The No-Cream Rule.** Quiet Fog is cool, not warm. If a background ever reads as cream, sand, or paper, it has drifted and must be corrected back toward neutral or graphite.

## 3. Typography

**Display Font:** single bold grotesque sans [font pairing to be chosen at implementation — must carry full Cyrillic support since all copy is Russian]
**Body Font:** the same family, lighter weight

**Character:** One typeface family doing all the work. Hierarchy comes from weight contrast (extra-bold display down to medium body) and scale jumps, not from mixing typefaces — the boldness itself is the "dерзкая типографика" machinescanthink.ai reference is pointing at.

### Hierarchy
- **Display** (800–900 weight, `clamp(2.5rem, 6vw, 6rem)`, line-height ~0.95, letter-spacing ≥ -0.04em): hero claims, section-opening statements.
- **Headline** (700 weight, `clamp(1.75rem, 3.5vw, 3rem)`, line-height 1.05): section titles.
- **Title** (600 weight, 1.25–1.5rem): sub-section and card-equivalent titles.
- **Body** (400–500 weight, 1–1.125rem, line-height 1.6, max 70ch): paragraph copy, bios, programme descriptions.
- **Label** (600 weight, 0.8125rem, letter-spacing 0.02em, sentence case): buttons and tags — explicitly not a tiny uppercase tracked eyebrow.

### Named Rules
**The One Family Rule.** Every weight in the system comes from the same grotesque sans. Richness comes from scale and weight jumps (≥1.25 ratio between steps), never from a second or third typeface.

## 4. Elevation

Flat by daylight default — no drop shadows on resting elements. Depth comes from alternating background blocks (Quiet Fog ↔ Cool Slate Mist) and from scale/whitespace jumps between sections, not from blur or shadow. Scroll-driven motion (entrances, transforms) carries the sense of depth that a shadow system would otherwise be asked to fake.

### Named Rules
**The Flat Daylight Rule.** No `box-shadow` on default elements. Depth is a function of which background block you're in, not how dark the blur under a card is.

## 5. Components

No components built yet — this is a seed file. Canonical primitives (buttons, nav, video-intro hero, contrast-block sections) will be documented here once implementation starts; re-run `/impeccable document` at that point to extract real tokens and generate the `.impeccable/design.json` sidecar.

## 6. Do's and Don'ts

### Do:
- **Do** keep Signal Orange (#ff9737) to one decisive use per screen — a primary CTA or a single highlighted insight, never a palette filler.
- **Do** build scroll-driven reveals and transforms for section entrances, each section visible-by-default with a `prefers-reduced-motion` crossfade fallback.
- **Do** alternate Quiet Fog (#eeeeee) and Cool Slate Mist (#d2dbda) background blocks section-to-section for contrast, instead of reaching for cards.
- **Do** let the single bold grotesque sans carry hierarchy through weight and scale, with display type up to `clamp(2.5rem, 6vw, 6rem)`.

### Don't:
- **Don't** introduce cream, beige, sand, or any warm near-white tone anywhere in the system — this is the explicit anti-reference to the "typical coach site."
- **Don't** use handwritten/script fonts, beach or lifestyle stock photography, or gradient-background quote cards.
- **Don't** default to a stiff, departmental-tile corporate-university layout, even though the brand is HSE-affiliated — this must read as Olga's personal authority, not an institutional page.
- **Don't** add countdown timers, loud multi-color CTA buttons, or "transformation in N days" urgency copy — the infobiznes/guru pattern PRODUCT.md explicitly rejects.
- **Don't** add a tiny uppercase tracked eyebrow above every section.
- **Don't** use `border-left`/`border-right` colored stripes as accents on cards or callouts; use full background-block contrast instead.
