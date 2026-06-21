# Design Prover MCP Server

Every AI frontend looks identical: hero, 3 cards, 3 cards, CTA, rounded-xl, shadow-lg, blue/gray/white. Design Prover forces the agent to prove its design has dramatic hierarchy, unpredictable layout, intentional whitespace, commanding typography, and color with actual personality.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/design-prover)

## Overview
**Category:** productivity
**Tools Count:** 1

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


## Installation & Usage

To install and use the **Design Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/design-prover](https://vinkius.com/mcp/design-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
