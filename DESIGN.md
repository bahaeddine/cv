---
name: Baha Eddine Boukhzar — CV
description: A precise, editorial cloud-engineer CV — warm stone-paper body pages bookended by two dark "night" sections.
colors:
  burnished-gold: "#82581F"
  burnished-gold-bright: "#D4AD5C"
  gold-signal: "#C79A3E"
  stone-paper: "#E4E3DC"
  stone-paper-raised: "#F2F1EA"
  ink: "#1B1B19"
  ink-dim: "rgba(27,27,25,0.64)"
  ink-faint: "rgba(27,27,25,0.64)"
  line: "rgba(24,24,22,0.13)"
  line-soft: "rgba(24,24,22,0.07)"
  night-ink: "#20211B"
  night-ink-raised: "#2B2C24"
  ivory: "#F3F0E6"
  ivory-dim: "rgba(243,240,230,0.68)"
  ivory-faint: "rgba(243,240,230,0.58)"
  line-night: "rgba(243,240,230,0.16)"
  line-night-soft: "rgba(243,240,230,0.08)"
typography:
  display:
    fontFamily: "Fraunces, Georgia, serif"
    fontSize: "clamp(48px, 8vw, 96px)"
    fontWeight: 500
    lineHeight: 1.02
  headline:
    fontFamily: "Fraunces, Georgia, serif"
    fontSize: "clamp(30px, 4vw, 44px)"
    fontWeight: 500
    lineHeight: 1.6
  title:
    fontFamily: "Fraunces, Georgia, serif"
    fontSize: "23px"
    fontWeight: 500
    lineHeight: 1.6
  caption:
    fontFamily: "Fraunces, Georgia, serif"
    fontStyle: "italic"
    fontSize: "15px"
    fontWeight: 400
    lineHeight: 1.6
  body:
    fontFamily: "Inter, -apple-system, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "Inter, -apple-system, sans-serif"
    fontSize: "13px"
    fontWeight: 500
    letterSpacing: "0.02em"
rounded:
  circle: "50%"
  pill: "999px"
  tooltip: "4px"
components:
  tag:
    backgroundColor: "transparent"
    textColor: "{colors.ink-dim}"
    rounded: "{rounded.pill}"
    padding: "5px 12px"
  nav-dot:
    backgroundColor: "#9A968A"
    rounded: "{rounded.circle}"
    size: "7px"
  nav-dot-active:
    backgroundColor: "{colors.gold-signal}"
    rounded: "{rounded.circle}"
    size: "7px"
  portrait:
    rounded: "{rounded.circle}"
    size: "112px"
---

# Design System: Baha Eddine Boukhzar — CV

## Overview

**Creative North Star: "The Night Editorial"**

Two dark, ink-black spreads — the opening hero and the closing contact section — frame a long, warm stone-paper interior, the way a print magazine profile opens on a bold cover treatment, settles into readable body pages, and closes on a deliberate final spread. The voice is precise, technical, and engineered rather than decorative: hairline rules, exact stat counts, and an italic-serif caption system do the work that a card grid or drop-shadow system would do elsewhere. Burnished gold is the single accent, held rare enough that its every appearance reads as a deliberate mark, not a color choice.

The system explicitly avoids the vocabulary of a generic SaaS/startup landing page (no card grids, no gradient buttons, no icon-in-a-circle feature blocks) and avoids a "flashy creative portfolio" register (no bold color blocking, no illustration, no playful motion). What replaces those is structure: a fixed side rail acting as a table of contents, hairline dividers standing in for containers, and a two-stage light/dark palette that does the framing a hero image or shadow system would otherwise do.

**Key Characteristics:**
- Two-stage palette: warm stone-paper body, ink-black hero/contact bookends.
- Fraunces serif (display/headline/title/caption) paired with Inter sans (body/label) — no third face.
- Gold used as a rare signal, never a fill: kickers, italic emphasis, active states, stat numbers.
- Depth via ambient glow and hairline rules, not drop shadows or card containers.
- A fixed dot-rail side nav functions as both navigation and a live scroll-position indicator.

## Colors

A near-monochrome stone-and-ink palette carries almost the entire page; a single warm gold is the only saturated color in the system, and it changes brightness by stage rather than by role.

### Primary
- **Burnished Gold** (`#82581F`): the accent on stone-paper (light) sections — kickers, italic "Boukhzar." emphasis, stat numbers, link-hover color, certification links. Darkened from an earlier `#A1752B` draft, which measured 3.2:1 against Stone Paper and failed WCAG AA on small text (kickers, verify links); this value holds 4.85:1.
- **Burnished Gold, Bright** (`#D4AD5C`): the same accent, raised in value for the two night sections (hero, contact) so it reads with equal weight against the dark ground.
- **Signal Gold** (`#C79A3E`): a third, slightly more saturated gold reserved for exactly one element — the active dot in the fixed side rail, which must stay legible as it crosses both light and dark backgrounds.

### Neutral — Stone-Paper Stage (body sections)
- **Stone Paper** (`#E4E3DC`): default page background for About, Experience, Skills, Certifications.
- **Stone Paper, Raised** (`#F2F1EA`): reserved raised surface (declared, not yet used by a component — keep for a future raised-panel need rather than introducing a new neutral).
- **Ink** (`#1B1B19`): primary text color on stone-paper.
- **Ink, Dim** (`rgba(27,27,25,0.64)`): secondary/body-paragraph text.
- **Ink, Faint** (`rgba(27,27,25,0.64)`): tertiary text — meta labels, timestamps, section summaries. Darkened from an earlier `0.42` alpha, which measured 2.52:1 against Stone Paper and failed WCAG AA; on this background the passing range for small text (≥0.627 alpha) sits almost on top of Ink, Dim's own value (0.64), so the two tiers now read as effectively one weight on the light stage — hierarchy between them here is carried by size and context, not opacity. The dark stage (below) still has enough range to keep a real third tier.
- **Line** (`rgba(24,24,22,0.13)`) / **Line, Soft** (`rgba(24,24,22,0.07)`): the two hairline-rule weights that do the dividing work cards would otherwise do.

### Neutral — Night Stage (hero, contact)
- **Night Ink** (`#20211B`): background for the hero and contact sections.
- **Night Ink, Raised** (`#2B2C24`): reserved raised surface for the night stage, mirroring Stone Paper Raised.
- **Ivory** (`#F3F0E6`): primary text on the night stage.
- **Ivory, Dim** (`rgba(243,240,230,0.68)`) / **Ivory, Faint** (`rgba(243,240,230,0.58)`): secondary/tertiary text on the night stage. Faint's alpha was raised from `0.44` (3.87:1, failed AA) to `0.58` (5.68:1) — this stage has enough contrast headroom to keep faint meaningfully lighter than dim while both clear 4.5:1.
- **Line, Night** (`rgba(243,240,230,0.16)`) / **Line, Night Soft** (`rgba(243,240,230,0.08)`): hairline rules on the night stage.

### Named Rules
**The Rare Gold Rule.** Gold never fills a shape — no gold buttons, gold backgrounds, or gold badges. It only marks: a kicker word, an italicized name, a stat number, an active dot, a hovered link. If gold would cover more than a few characters or a 7px dot, it's being used wrong.

**The Bookend Rule.** The night palette is reserved for the hero and contact sections only. Every section in between stays on the stone-paper stage. A third dark section would break the "cover and closing spread" structure the system depends on.

## Typography

**Display Font:** Fraunces (with Georgia, serif fallback)
**Body Font:** Inter (with -apple-system, sans-serif fallback)

**Character:** Fraunces' high-contrast, slightly quirky serif carries every moment of emphasis and identity (the name, section heads, the italic kicker caption); Inter stays completely neutral underneath it for body copy and labels, so the serif is never competing with a second expressive face.

### Hierarchy
- **Display** (500, `clamp(48px, 8vw, 96px)`, line-height 1.02): the name on the hero — the only place line-height is tightened off the base rhythm.
- **Headline** (500, `clamp(30px, 4vw, 44px)`): every section's `h2.head` — About's headline runs a slightly smaller clamp (`clamp(26px, 3.4vw, 38px)`) because its copy is a full sentence rather than a short label.
- **Title** (500, 23px): company/role names in the experience list (`.exp-company`).
- **Caption** (400 italic, 15px, Burnished Gold): the kicker line above every section headline ("Who I am", "Where I've worked") — Fraunces' one italic use in the system.
- **Body** (400, 16px, line-height 1.6, max ~56ch): paragraph copy; the hero tagline runs at 18px, everything else at 16px.
- **Label** (500, 13px, letter-spacing 0.02–0.03em): nav labels, the hero eyebrow, meta-row text — always uppercase-adjacent in weight even when not uppercased.

### Named Rules
**The One-Italic Rule.** Italic Fraunces is reserved for kickers and the single emphasized word in the hero name ("*Boukhzar.*"). It never carries a full sentence or paragraph.

## Layout

A fixed 78px-wide dot-rail occupies the left edge on desktop (≥821px) and doubles as a scroll-position indicator; below 820px it's replaced by a sticky, horizontally-scrollable top nav bar (translucent stone-paper, blurred backdrop, hairline bottom border) carrying the same six section links, and sections lose their left padding, becoming a single readable column. Content is capped at `max-width: 1040px` inside a `.wrap` container with 40px horizontal padding.

Section rhythm is consistent and generous: `130px` top padding, `40px` bottom padding, `78px` left padding (desktop), each section opening with a hairline top border (`line-soft`) rather than a background change — the seams are visible, not hidden. Two-column moments (`.about-grid` at 1.4fr/1fr, `.exp-role` at 220px/1fr) collapse to a single column at 820px and 640px respectively. `html { scroll-behavior: smooth }` plus an IntersectionObserver-driven `.reveal` fade/slide (24px translate, 0.7s ease) animates each section's content in on scroll, disabled under `prefers-reduced-motion`.

## Elevation & Depth

The system is flat by default — no card containers, no elevation scale, no drop shadows on content blocks. Depth is conveyed two other ways: an ambient, animated radial-gradient "glow" and "halo" behind the hero copy and portrait (soft-focus light, not a shadow, pulsing slowly via `glowpulse`/`drift` keyframes), and exactly one true shadow in the entire page — a small lift under the circular portrait (`0 6px 22px rgba(27,26,22,0.14)`) plus a matching soft ring around the active nav dot (`0 0 0 3px rgba(128,124,112,0.18)`). Everything else sits directly on its background, separated by hairlines rather than boxes.

### Shadow Vocabulary
- **Portrait lift** (`box-shadow: 0 6px 22px rgba(27,26,22,0.14)`): the only structural shadow — grounds the circular headshot.
- **Active-dot ring** (`box-shadow: 0 0 0 3px rgba(128,124,112,0.18)`): a soft halo confirming the current nav position, not a lift.

### Named Rules
**The Flat-By-Default Rule.** Sections, tags, and text blocks carry no shadow. If something needs to feel "raised," reach for the ambient glow treatment or a hairline border before reaching for `box-shadow`.

## Shapes

Corners are binary and deliberate: perfectly circular for the portrait and nav dots (`border-radius: 50%`), full pill (`999px`) for skill tags, and a single small `4px` radius for the nav-label tooltip — nothing in between. Sections, the `.wrap` container, contact rows, and experience rows are all sharp-cornered rectangles; the system never reaches for an 8–16px "card radius." Borders, where they exist, are always 1px hairlines in `line`/`line-soft` (or their night-stage equivalents), never a heavier stroke.

## Components

### Chips (Skill Tags)
- **Style:** transparent background, 1px `line` border, `999px` pill radius, `ink-dim` text at 13px, `5px 12px` padding.
- **State:** static — no selected/unselected variants; tags are informational, not interactive.
- **Responsive:** each category (`.skill-cat`) is a 190px label beside a wrapping tag row; below 640px it stacks (`flex-direction:column`, label width auto), matching the collapse convention `.about-grid` and `.exp-role` already use at their own breakpoints.

### Hero Stat Strip
- **Style:** a compact, inline version of the About section's stat-list — small serif numerals (`28px`, Fraunces 500, gold) over a 12px label (`ink-faint`) — placed between the tagline and the meta-row so the page's two headline credibility numbers (scope and tenure) land inside the first viewport instead of only after a scroll into About.
- **Relationship to the full stat-list:** intentionally a subset (2 of the 3 About numbers) and a smaller scale — it previews the proof, About still delivers the full picture, so the hero doesn't have to choose between identity and evidence.

### Navigation
- **Side rail (desktop):** a vertical stack of 7px dots (`#9A968A` at rest, Signal Gold `#C79A3E` and 1.5x scale when active) with a dark pill tooltip label that fades/slides in on hover (`opacity 0→1`, `translateX(-6px→0)`). Fully hidden below 820px.
- **Mobile top nav (below 820px):** a sticky, horizontally-scrollable bar of six text links (13px, `ink-dim`, gold border-bottom on hover/focus) on a translucent stone-paper ground with `backdrop-filter: blur(8px)` and a hairline bottom border — gives mobile the same persistent, from-anywhere wayfinding the dot-rail gives desktop, instead of relying solely on the trailing quicknav.
- **Footer quicknav:** a flat wrapped list of text links (13.5px, `ink-dim`, gold on hover) — a secondary, end-of-page link list; the mobile top nav is what carries wayfinding responsibility during the scroll.

### Links
- **Style:** inherit color, no underline at rest; a 1px bottom border appears and text shifts toward gold on hover (`border-color`/`color` transition, 0.2–0.25s). Applies uniformly to meta-row links, the phone contact row, certification "verify" links, and the footer contact link.
- **Primary email link (signature emphasis):** the one deliberate escalation in the system — the contact section's email address alone jumps to display-adjacent scale (`clamp(28px, 3.6vw, 40px)`, Fraunces 500) with a permanent 2px gold underline (not hover-only), following the small-label-beside-big-value grammar already established by the stat-list. It's the page's one conversion moment, so it's the one link allowed to outweigh its neighbors; no other link in the system gets this treatment.

### Accordion Experience Row (signature)
- **Structure:** a header button (`.exp-top`, a real `<button>` for native keyboard operability — company + date range + a serif "＋" toggle glyph, `aria-expanded`/`aria-controls` wired to its body) above a body that animates open via `max-height: 0 → 900px` over 0.5s ease; only one entry (Renault Group, the current role) starts open. Without JavaScript, all bodies render fully expanded rather than clipped shut, so the content stays reachable either way.
- **Content:** stacked role blocks inside, each with a 220px/1fr meta/detail grid (collapsing to one column at 640px), separated by soft hairlines when a company has multiple roles.
- **Character:** deliberately unhurried — no chevron rotation or spring easing, just a calm height expansion consistent with the system's restrained motion vocabulary.
- **Continuity thread (`.exp-body--threaded`, multi-role companies only):** a 7px dot (rest `#9A968A`, current role `gold`, reusing the side-rail's exact dot vocabulary) beside each role, connected by a 1px `line` hairline running down through the block — the one company with more than one role (Renault) reads visually as a single continuous thread, distinct from how the single-role peer companies render below it as plain unconnected rows. The ongoing role also carries an `11px` uppercase "Current" label in gold next to its title, so the distinction never depends on dot color alone.

### Named Rules
**The Told-and-Shown Rule.** A claim PRODUCT.md calls a genuine differentiator (not just a fact) gets a structural visual device, not only prose — continuity is a sentence in the About copy *and* a connected thread in the Experience accordion; a fact that's merely true doesn't need the second treatment.

## Do's and Don'ts

### Do:
- **Do** treat gold as a mark, not a fill — kickers, one italic word, stat numbers, hover states, the active nav dot (**The Rare Gold Rule**).
- **Do** keep the dark palette to exactly the hero and contact sections; every section between them stays on stone-paper (**The Bookend Rule**).
- **Do** use hairline borders (`line`/`line-soft`, or their night-stage equivalents) as the default way to separate content — reach for a divider before reaching for a container.
- **Do** let Fraunces own every display/headline/title/caption moment and keep Inter to body copy and labels — no third typeface.

### Don't:
- **Don't** add `box-shadow` or card-style containers to content sections — depth comes from the ambient glow treatment and hairlines only (**The Flat-By-Default Rule**).
- **Don't** introduce a filled or bordered gold button — no component in this system uses gold as a background color.
- **Don't** round corners beyond the established set (circle, 999px pill, 4px tooltip) — there is no card-radius aesthetic to extend.
- **Don't** set full paragraphs or multi-word headings in italic Fraunces — italic is reserved for kickers and single-word emphasis (**The One-Italic Rule**).
