# Design Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/design-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Every AI frontend looks identical: hero, 3 cards, 3 cards, CTA, rounded-xl, shadow-lg, blue/gray/white. Design Prover forces the agent to prove its design has dramatic hierarchy, unpredictable layout, intentional whitespace, commanding typography, and color with actual personality.

## Description
Tell an AI agent to build a landing page and you know exactly what you'll get: centered hero with gradient background, three feature cards in a row, three testimonial cards, pricing table with the middle plan highlighted, four-column footer. rounded-xl on everything, shadow-lg on the cards, gap-6 between them, bg-white/bg-gray-50, blue-600 buttons. Every. Single. Time.

The problem is deeper than aesthetics. AI agents don't DESIGN — they ASSEMBLE. They reach for the same layout skeleton, the same component library patterns, the same safe color palette. The result looks "professional" the way a stock photo looks "happy" — technically correct, emotionally void.

### The 5 AI Design Fingerprints

1. **Flat hierarchy** — every element has the same visual weight. Headlines are 2x body when they should be 5x. No focal point, no reading path, no drama.
2. **Card-grid addiction** — hero → 3 cards → 3 cards → CTA. The universal AI skeleton. No asymmetry, no overlapping, no broken grids, no spatial tension.
3. **Uniform spacing** — gap-6 everywhere, p-4 on everything. No contrast between dramatic emptiness and tight clusters. Space is padding, not design.
4. **Muted typography** — one font (Inter or system), predictable size scale (text-sm through text-5xl). No dramatic ratio, no display fonts, no type as visual element.
5. **Safe palette** — blue/indigo primary, gray neutrals, white background. The "startup kit." Zero personality, zero brand identity.

### How Design Prover Works

5 Decision Pivots force the agent to prove intentional design before writing HTML:

1. **hierarchyDramatic** — Name the ONE element that dominates. 3:1+ size ratio between primary and secondary. Clear reading path from focal point to detail.
2. **layoutUnpredictable** — No card grids. Asymmetric columns, overlapping elements, full-bleed sections contrasting with narrow text, alternating dense and sparse.
3. **whitespaceDesigned** — 200px of emptiness next to 4px-gap data clusters. The variation between generous and tight IS the design.
4. **typographyCommands** — 72px display + 14px body = 5:1 ratio. Mixed families (serif display + sans body). Weight contrast (900 vs 300). Specific px values, not Tailwind defaults.
5. **colorHasIdentity** — Specific hex values with intentional mood. Dark charcoal + electric cyan = cyberpunk. Off-white + burgundy = editorial luxury. Not "blue because professional."

### The Core Insight

Professional design is made of DECISIONS. AI assembles defaults. Every rounded-xl, every shadow-lg, every gap-6 is a default the agent reached for instead of deciding. Design Prover forces five concrete decisions: what dominates, how space flows, how type commands, why these colors, where the eye goes. Decisions produce design. Defaults produce templates.


## Available Tools
- **prove_design**: Every AI-generated frontend looks the same because AI defaults to the same skeleton: safe colors, uniform spacing, card grids, single font family. Your job is to design with INTENTION, not defaults. You must: (1) name the FOCAL POINT — ONE element that visually dominates with 3:1+ scale ratio. Not "the hero section" — that is a container. Name the specific element, its size, and why the eye goes there first. If nothing commands attention, the design is flat, (2) describe the LAYOUT — no card grids. Each section must have a DIFFERENT spatial relationship. Asymmetric columns, overlapping elements, full-bleed sections, alternating dense/sparse. If you can describe it as "N cards in a row," redesign, (3) map the WHITESPACE — where is space dramatic (160px+)? Where is it tight (4px)? Uniform padding is uniform boredom. The variation between generous and tight IS the design, (4) define the TYPOGRAPHY — specific sizes (px/rem), font pairings, weight contrasts. Minimum 3:1 ratio between largest and body. Mixed families create character. Weight contrast (900 vs 300) creates tension, (5) justify the COLOR — why these specific hex values? What personality do they create together? The RELATIONSHIP between colors is the identity. Blue/gray/white is not an identity, (6) name a REFERENCE — a specific site AND the specific design choice you are borrowing. Not "Apple" or "minimalist" — those describe a decade. "Linear.app — motion for state transitions." If rejected, your frontend will look like every other AI-generated page.

Structured reflection tool that forces the agent to PROVE its frontend design breaks AI-generated patterns before writing HTML/CSS. AI frontends follow the same skeleton: hero → 3 cards → 3 cards → CTA, rounded-xl, shadow-lg, gap-6, blue/gray/white. This tool catches that skeleton and forces intentional design. Catches Flat Hierarchy (no element dominates — everything is the same size, weight, and color. The eye wanders without a focal point. If nothing commands attention, the design is flat), Card Grid (hero → 3 cards → 3 cards → CTA. If you can describe the layout as "N cards in a row," it is the AI default skeleton — every AI-generated page looks identical), Uniform Spacing (same padding and gap everywhere — gap-6, p-8, rounded-xl on repeat. The VARIATION between generous whitespace and tight clusters IS the design), Muted Typography (text-sm to text-5xl with one font family. No drama. 72px display + 14px body = 5:1 ratio = hierarchy. Default scale = default boredom), and Safe Palette (blue/gray/white — the AI startup kit. If you can swap the logo and the page looks like any other SaaS landing page, the palette has no identity). Call once per frontend design before writing any HTML/CSS


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Design Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Build a landing page for a project management SaaS. Make it modern and clean with feature cards."

**🤖 AI Agent:**
> Multiple rejections. (1) FLAT_HIERARCHY — what dominates? (2) CARD_GRID — 'feature cards' is the AI skeleton. (3) 'Modern and clean' describes every AI design ever made. What does this FEEL like? A cockpit? A magazine? Name the emotion, the density, the unexpected element. Redesign before writing code.

---

**👤 You:**
> "Focal: metric '99.97%' at 96px mono bold on #0a0a0f. Layout: full-bleed dark hero, asymmetric 65/35 below, single-column manifesto section. Type: 96px/Jetbrains Mono + 15px/Inter. Color: #0a0a0f + #00d4ff cyan accent + #1a1a2e surfaces."

**🤖 AI Agent:**
> Verdict: DESIGN_READY. Hierarchy: 96px metric vs 15px body = 6.4:1 ratio. Layout breaks grid: full-bleed hero, asymmetric columns, manifesto section. Whitespace contrast present. Type: two families (JetBrains Mono + Inter), dramatic scale. Color: dark + cyan = technical/premium. This design has decisions, not defaults. Build it.

---

**👤 You:**
> "Focal: hero headline. Layout: hero + 3 feature cards + pricing. Type: text-xl to text-4xl. Color: blue-600 primary, gray-100 background."

**🤖 AI Agent:**
> 5 rejections. (1) FLAT_HIERARCHY — 'hero headline' is vague. Size? Font? Ratio? (2) CARD_GRID — 'hero + 3 cards + pricing' is the AI skeleton verbatim. (3) UNIFORM_SPACING — no whitespace contrast specified. (4) MUTED_TYPE — text-xl to text-4xl is Tailwind defaults, not design. (5) SAFE_PALETTE — blue-600 + gray-100 is the universal AI color kit. Fix all five.


## ❓ FAQ

**Q: Does Design Prover generate HTML or CSS?**
No. Design Prover generates zero code. It forces the agent to make five concrete DESIGN DECISIONS — hierarchy, layout, whitespace, typography, color — before writing a single line of HTML. The decisions then guide the code. The tool catches AI patterns (card grids, uniform spacing, safe palette) and rejects until the design is intentional.

**Q: Why does it reject card grids?**
Three cards in a row is the #1 fingerprint of AI-generated design. It's the default every model reaches for because it's safe and symmetrical. Professional design uses spatial tension: asymmetric columns where one is 2x wider, elements that overlap or break containers, full-bleed images next to narrow text columns, alternating between dense data sections and generous white space. Card grids are assembly, not design.

**Q: What does a 3:1 hierarchy ratio mean?**
If your body text is 16px, your focal element should be at least 48px (3x) to create real visual dominance. AI agents typically use 32px headlines with 16px body — a 2:1 ratio that creates no drama. Professional design uses 5:1+ ratios: 72px display headlines, 120px metrics, oversized imagery. The bigger the ratio, the clearer the reading path.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/design-prover](https://vinkius.com/mcp/design-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Design Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `design-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Design Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "design-prover": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
