# PoolGo Brand

## Positioning

PoolGo is the home for everything about your pool: water, equipment, service, and the people who help you keep it running.

We're not a directory. We're not a marketplace. We're the place where everything your pool needs to be remembered actually gets remembered.

## Audience

**Primary**: pool-owning homeowners, mid-30s to 60s, suburban, comfortable with apps but not technical. Already paying a service company or testing their water at a local pool retail store.

**Jobs to be done**:
1. "Tell me if my pool is okay right now."
2. "Remember everything my pool store told me last visit."
3. "Connect me to someone good when something breaks."
4. "Help me not screw it up."

**Secondary**, deferred to later phases:
- Pool retail stores (data source for water tests)
- Service pros (Discover supply side; their primary product is PoolrouteOps)

## Brand Pillars

Three attributes that should be visible in every pixel and every line of copy.

### Warm
The app feels like a friendly neighbor, not a utility.
- Rounded geometry, generous radii.
- Photography of real pools, real hands, real golden-hour moments.
- Language without jargon.

### Confident
We know pools.
- We make recommendations, not endless tooltips.
- Real numbers, not gauges with vague "good/bad" colors.
- Plain-language verdicts: "Your chlorine looks good. No action needed today."

### Calm
Pool care is supposed to be relaxing.
- Generous whitespace.
- Restraint with red and yellow. Status colors only earn their saturation when something is genuinely off.
- No pop-ups. No countdown timers. No "X people are looking at this pro right now" growth-hacks.

## Voice

**Friendly, plainspoken, second-person.** Says "your pool" not "the asset."

**Confident without being clinical.** Says "Free chlorine looks good" not "FC: 2.4 ppm, within nominal range." Lab numbers are present, but in service of the verdict, not in place of it.

**No em-dashes anywhere.** Use commas, periods, parentheses.

**No hype words.** Banned: revolutionize, seamless, powerful, unlock, transform, leverage, supercharge, next-generation.

**Headline + descriptor pattern.** Short headline that states a fact. Descriptor that adds the "so what." Example:
> Your pool, all in one place.
> Track your water, connect your equipment, find a pro you trust.

## Visual System

### Color

| Token | Hex | Role |
|-------|-----|------|
| Cream | `#FAF6EF` | Primary surface. Page background. The brand's most-used color. |
| Cream Deep | `#F2EBDD` | Hover states, alt rows, deep-cream surfaces. |
| Pool | `#2E8C9C` | Hero blue. Primary buttons. Active states. The pool itself. |
| Pool Deep | `#1F6772` | Pool hover. Dark accents on cream. |
| Pool Tint | `#D5E5E8` | Pool background tints. Chart fills. Pills. |
| Deep | `#0F2A33` | Primary text. Footer surface. Active tab fill. |
| Deep Soft | `#2E4951` | Body copy on cream. |
| Deep Mute | `#5A6F77` | Subtle copy, captions, label text. |
| Sun | `#E8B956` | Accent. Highlights, sun-CTA, selected nav, chart accents. |
| Sun Deep | `#C7973A` | Sun hover. |
| Clay | `#C8745A` | Secondary accent. Avatars, illustrations, warmth moments. |
| Mist | `#E4EBEC` | Dividers, gridlines, card borders. |
| Mist Deep | `#C8D3D6` | Form borders. |

**Semantic colors are desaturated 20% from typical web defaults** so the calm pillar holds:

| Status | Hex | Notes |
|--------|-----|-------|
| Good | `#6FA178` | Use for in-range readings, healthy states. |
| Warn | `#D9A648` | Use for nearing-out-of-range. Same family as Sun on purpose. |
| Error | `#C25C53` | Use only when something is genuinely wrong. |

**Rule**: a parameter is shown in `Good` only if the homeowner can think *"that's good"* without reading text. Mid-range chemistry is `Neutral` (no color), not `Good`.

### Typography

**Display: Fraunces.** Variable serif with optical sizing. Used for hero, headers, big stats. Optical-size axis lets us go wide and warm at display sizes, tight and confident at body sizes. Already in our system, kept on purpose.

**Body: Inter.** Humanist sans replacing Plus Jakarta Sans. Slightly less geometric, slightly more humanist. Better for long-form reading. Wide installed-base reliability.

**Mono: JetBrains Mono.** For chemistry readings, telemetry values, anything that should feel like it came off a real instrument. Tabular figures (`font-feature-settings: 'tnum'`) so values align in tables.

**Type scale** (`tokens.css` is authoritative):

| Role | Size | Use |
|------|------|-----|
| Hero | clamp(2.75rem, 5.2vw, 4.75rem) | Homepage hero only. |
| Display | clamp(2rem, 3.5vw, 3rem) | Section headers. |
| H1 | clamp(1.625rem, 2.5vw, 2.25rem) | Page titles. |
| H2 | clamp(1.25rem, 1.8vw, 1.5rem) | Card titles. |
| Stat | clamp(3.5rem, 7vw, 5.5rem) | The hero stat in My Pool dashboard. |
| Body | 1rem | Default. |
| Small | 0.875rem | Captions, secondary copy. |
| Tiny | 0.75rem | Labels, eyebrow text. |

### Logo

Three concepts to choose from. Mocks default to **Concept A (wordmark only)** for the cleanest read; swap once a final mark is selected.

#### Concept A — Wordmark only
```
Pool Go
```
- "Pool" in Fraunces semibold, Deep `#0F2A33`.
- "Go" in Fraunces semibold italic, Pool `#2E8C9C`.
- Tight kerning (-0.025em).
- No mark, no chip, no container.
- Best for: a brand that earns its trust with consistency, not with logo gymnastics. Most lifestyle brands we admire (Hims, Topo Chico, Aesop wordmarks) sit in this family.

#### Concept B — Wordmark + dot motif
- Same wordmark.
- The two **o**'s in "Pool" carry an inner ring at 0.4× radius, evoking pool tile or a tinted droplet.
- Subtle. Reads as a wordmark at small sizes.
- Best for: a slightly more proprietary mark without committing to a separate logomark. Works at favicon scale (single `o`-with-ring).

#### Concept C — Wordmark + abstract mark
- Wordmark plus a curved-line mark to its left: a single horizontal line of water surface with a subtle ripple.
- The mark reads as "the surface of your pool."
- Best for: a brand that wants a separate mark for app icons, social avatars, partnership lockups.

**Decision rule**: pick A if you want PoolGo to feel like a confident lifestyle brand. Pick B if you want a small piece of personality without a real mark. Pick C only if you can commit to drawing the mark in 8 sizes (favicon, app icon, business card, signage, etc.).

**Things to avoid**:
- The current "PG" rounded-square chip. Reads as 2018 startup template.
- Gradients in the mark.
- Anything that needs a colored container behind it to read. The wordmark must hold on Cream and on Deep.

### Iconography

- Stroke-based, ~1.5px weight at 24px size.
- Rounded line caps and joins.
- Slight off-grid imperfection where it serves warmth (a 23-degree angle where a 22.5 would be "correct" by the icon-grid orthodoxy).
- **Reference**: Phosphor "duotone" set, hand-drawn sets like Streamline Sketch.
- **Avoid**: Material filled icons, glyph icons that read as buttons, icon sets with strict 90/45-degree rules.

### Imagery

- Real photography. Real pools. Real hands.
- Time of day: golden hour or just after.
- Crop tight. Pool tile macro shots. Water surface textures. Hands holding test strips.
- One person in frame at a time, max. Family is implied, not staged.
- **Avoid**: stock photography of "happy diverse families by aqua-blue resort pool." Stock illustration of geometric blob people. Drone shots of suburbia.

### Components

Defined in `mocks/tokens.css` and used in all three mocks.

- **Button** — Pill (`border-radius: 999px`). Primary fills Pool, text Cream. Secondary fills Cream with Mist Deep border, text Deep. Tertiary is text-only Pool.
- **Card** — `radius-lg` (16px), Cream-tinted-white background, `shadow-sm` (4-layer subtle shadow), `1px` border at `rgba(15, 42, 51, 0.04)`.
- **Stat** — Fraunces variable at large size, Mono unit suffix, label in tiny uppercase Inter above.
- **Reading row** — Three columns: parameter name (Inter small, Deep Soft), mono value, status pill. Bottom border `Mist`.
- **Pill** — Pill radius, tiny font, +0.04em letter-spacing. Six variants: good / warn / error / neutral / pool / sun.
- **Top nav** — Sticky, blurred Cream background (~85% opacity), Mist bottom border. Wordmark left, segmented tabs in a Cream Deep pill center, Avatar right.

### Motion

Stated as principles only. Implementation deferred until we move into Next.js.

- **Calm easings.** Default ease: `cubic-bezier(0.16, 1, 0.3, 1)`. Avoid bounces.
- **No parallax.**
- **No auto-playing video.**
- **Page transitions.** A small Y-offset fade (8px, 260ms) is enough.
- **Hover states.** Subtle. 1px translate, color shift. No scaling above 1.02.

## What we explicitly do NOT do

- No hero gradients. The current poolgo.co cyan→navy gradient is the vibe we're rejecting.
- No "Verified ✓ / Trusted ✓ / 5-Stars ✓" trust-badge rows. Trust is earned by design quality.
- No emoji in the UI.
- No corporate-tech-startup illustrations (geometric blob people, isometric "platforms").
- No pop-ups. No interstitials. No "We use cookies" maximalism (a small, dismissable banner is fine).
- No ALL CAPS marketing copy. ALL CAPS is reserved for tiny eyebrow labels (≤ 14px).

## Layout system

- Page background: **Cream** (`#FAF6EF`).
- Card surfaces: **White** with subtle Cream undertone, 16px radius.
- Container max width: 1200px. Prose max width: 640px.
- Gutter: `clamp(1.25rem, 4vw, 3rem)`.
- Section padding: 6rem top/bottom (`--space-9`).
- Vertical rhythm: 8px base unit. Spacing tokens in 4px increments up to 8rem.

## Surface-specific notes

### Marketing homepage
- Cream throughout. Deep band only at the footer.
- Hero is quiet. One headline, one descriptor, one primary CTA, one tertiary link.
- Below the fold: three "what PoolGo does" tiles (Chart / Connect / Routines), then a "remembered visit" band, then a "find a pro" band, then a small For-Pros band, then footer.

### My Pool dashboard
- The single most important screen.
- Default authenticated landing.
- Hero stat: today's most-relevant water reading (Free Chlorine), giant Fraunces number, plain-language verdict.
- Sub-stats grid: pH, TA, CYA, Salt.
- 30-day chart: FC primary line in Pool, pH overlay in Sun. Mist gridlines.
- Equipment glance: 2-3 device cards.
- Routines glance: 2 active routines with last-triggered time.
- "From your pool store": a quote-card mimicking what a retail tech said at the last visit.

### App shell
- Same top nav as dashboard.
- Five surface tabs: My Pool / Chart / Connect / Routines / Discover.
- Each tab demonstrates the brand carries across that surface without forcing.

## What's NOT in this brand exercise

- Backend models, MCP server, ClearCare ingestion, real telemetry. All deferred.
- Real photography (we're using Unsplash placeholders in the mocks).
- Mobile-app design (web only for this exercise; mobile is a follow-on).
- Marketing copy beyond the homepage (no email templates, no pricing page, no help center).
- The PoolrouteOps brand (lives separately, federates later).
