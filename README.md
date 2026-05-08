# PoolGo brand mocks

Standalone HTML/CSS mocks for the PoolGo consumer surfaces, in the **Pure** brand direction.

These are throwaway-cheap iterations meant for review before porting into the real Next.js frontend at `Poolify-us/poolgo`. No JS frameworks. Vanilla CSS. Inter Tight + real OEM brand colors as the design system.

## Live preview

The six consumer surfaces, all in the Pure direction:

- **My Pool** (Command Center) — https://rkurani.github.io/poolgo-mocks/mocks/screen-cmd-showroom-pure.html
- **Care** (MyChart-for-pools) — https://rkurani.github.io/poolgo-mocks/mocks/screen-care-pure.html
- **Equipment** (grid by Spaces) — https://rkurani.github.io/poolgo-mocks/mocks/screen-equipment-pure.html
- **Routines** (Alexa-style + AI builder) — https://rkurani.github.io/poolgo-mocks/mocks/screen-routines-pure.html
- **Folks** (Discover / Yelp-of-pool) — https://rkurani.github.io/poolgo-mocks/mocks/screen-discover-pure.html
- **Inbox** (unified messages) — https://rkurani.github.io/poolgo-mocks/mocks/screen-inbox-pure.html

## Brand reference

- [DESIGN.md](DESIGN.md) — the canonical design system in Google Labs's open DESIGN.md format. YAML tokens + 8 prose sections. Agents (Claude Code, Cursor, Stitch) read this as the contract.
- [BRAND.md](BRAND.md) — earlier prose-only brand spec. DESIGN.md supersedes the visual sections; BRAND.md still holds positioning and voice.
- [mocks/architecture.html](mocks/architecture.html) — the IA reference: 4 categories, 6 surfaces, 4 tile shapes, mapping of existing mocks.

## What's locked

The three Pure-brand surfaces above share:

- **Pure white surface** with `#FAFAFA` / `#F5F5F4` neutrals
- **Inter Tight** at 700–800 weights for display, 500 for body
- **OEM color inheritance** per card via `data-brand` attribute. Each equipment card / store card / pro card carries the brand color of who made or owns it (Pentair blue, Hayward yellow, Polaris teal, Sun Country gold, Leslie's royal blue, Marina forest, etc.).
- **PoolGo cyan** (`#1FA0BF`) only as accent — the wordmark dot, AI band glow, the You-pin on the map.
- **4-source legend** for Care: Live (sage), Imported (gold), Human (coral), AI (cyan).

## Other directions in the repo

`mocks/` also contains earlier explorations (Pool Club editorial, Field Notebook, Showroom dark, Iter 1/2/3) that we passed on. Kept for reference. The Pure files are the locked direction.
