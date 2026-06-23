# Tailwind Excellence Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tailwind-excellence-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

AI agents build bloated styling layers containing arbitrary values, div-only layouts, inaccessible contrast, and legacy configurations. This prover enforces strict design token structures (@theme), utility-first compliance, semantic HTML, mobile-first layouts, and interactive focus states.

## Description
Generating utility-first styles without strict design token constraints results in visual inconsistency, bloated files, and inaccessible web experiences. This tool analyzes class declarations to guarantee compliance with modern design system architecture.

### The Problem

Tailwind stylesheets often suffer from five major implementation failures:

- **Token Detachment** — Hardcoding random hex colors or arbitrary pixel sizes instead of using custom `@theme` variables.
- **Arbitrary Value Abuse** — Overusing classes like `w-[347px]` or `text-[#e74c3c]` for elements that should map to consistent design scales.
- **Div-Soup Layouts** — Ignoring semantic HTML markup (`<main>`, `<nav>`) and leaving interactive elements without clear focus indicator states.
- **Desktop-First Hardcoding** — Designing views for wide viewports and overriding layout behavior instead of building mobile-first scales.
- **Legacy v3 Anti-patterns** — Maintaining `tailwind.config.js` setups instead of adopting clean v4 CSS-based `@theme` declarations.

### How It Works

5 Decision Pivots validate the CSS structure:

1. **designTokensUsed** — Ensures all utility values reference custom `@theme` scale tokens.
2. **noArbitraryAbuse** — Restrains inline arbitrary classes to one-off alignments, enforcing scales.
3. **accessibilityMet** — Verifies focus rings, screen-reader text, color contrast, and keyboard navigation.
4. **responsiveMobileFirst** — Enforces base-mobile scaling overrides using progressive screen breakpoints.
5. **componentStructureClean** — Audits class ordering patterns, state variants, and utility file extractions.


## Available Tools (1)
- **validate_tailwind_excellence**: PILLAR I — DESIGN SYSTEM: Tailwind v4 uses @theme in CSS (NOT tailwind.config.js). Define tokens: --color-primary/secondary/danger (50-950 scale), --spacing-* (4px base), --font-heading/body, --radius-sm/md/lg. Dark mode via dark: variant or color-scheme. NEVER abuse arbitrary values ([347px], [#e74c3c]) — if used >1x it belongs in @theme. PILLAR II — ACCESSIBILITY: semantic HTML (header/main/nav/section, NOT div soup), aria-label on icon buttons, alt on images, sr-only for screen readers, focus-visible:ring-2 on EVERY interactive element, 4.5:1 contrast ratio, motion-safe:/motion-reduce: for animations. PILLAR III — RESPONSIVE: Mobile-first (base=mobile, sm:/md:/lg: upward). Grid: grid-cols-1 md:grid-cols-2 lg:grid-cols-3. @container for component-level responsive. Fluid typography. Touch targets ≥44px. TAILWIND v4: @import "tailwindcss" (no @tailwind directives), @theme for tokens, @utility for custom utilities, @variant for custom variants, automatic content detection. If rejected, fix the design violation.

Structured reflection for Tailwind CSS v4 excellence — forces systematic validation across three pillars: design system integrity, accessibility compliance, and responsive mastery. Built from Tailwind v4 architecture (@import "tailwindcss", @theme block, @utility, @variant, automatic content detection — NOT the legacy tailwind.config.js approach). Catches Arbitrary Value Abuse (using [#e74c3c] and [347px] instead of design tokens — a component uses bg-[#e74c3c] for error states. Searched the codebase: appears 14 times. Another component uses text-[#e74c3c]. A third uses border-[#e74c3c]. 14 occurrences of a hardcoded hex value. If the brand color changes: 14 places to update. One is missed. Now the error state is #e74c3c in 13 places and #e74c4c (typo) in 1 place. Fix: @theme { --color-danger: #e74c3c; } then bg-danger, text-danger, border-danger everywhere. 1 place to update. 0 risk of inconsistency. Rule: if an arbitrary value appears more than once, it belongs in @theme. Acceptable arbitrary use: one-off alignment like top-[3px] that is truly unique), Div Soup (47 nested <div> elements, zero semantic HTML — a pricing page: <div> for header, <div> for nav, <div> for main, <div> for cards, <div> for card content, <div> for footer. 47 divs total. Screen reader announces: "group, group, group, group, group..." — meaningless. Google cannot determine content structure — no article, no section, no heading hierarchy. Fix: <header> for page header, <nav> for navigation, <main> for primary content, <section> for pricing tiers, <article> for each plan, <footer> for page footer. Same Tailwind classes. Completely different semantic meaning. Screen reader: "banner, navigation, main, region: pricing, article: Pro Plan, contentinfo." Semantic HTML costs zero effort — it is choosing the RIGHT element instead of the wrong one), Desktop-First Responsive (writing base styles for desktop and overriding downward — component: grid-cols-3 sm:grid-cols-1. Problem: sm: means "640px and UP" in Tailwind. This is NOT "make it 1 column on mobile." This says: "3 columns at all sizes, then 1 column at 640px+" — the OPPOSITE of intent. On mobile (< 640px): 3 columns. Completely broken layout. Horizontal scroll. Unusable. Fix: grid-cols-1 md:grid-cols-2 lg:grid-cols-3. Base = mobile (1 column). md: = tablet (2 columns). lg: = desktop (3 columns). Mobile-first means: base styles ARE mobile. Breakpoints ADD complexity upward. If you write grid-cols-3 FIRST: you are thinking desktop-first — and mobile is broken), Accessibility Theater (icon-only buttons without aria-label, missing focus states — a delete button: <button class="p-2"><TrashIcon /></button>. Visually: a trash icon. Clear to sighted users. Screen reader: "button." That is all. No label. The user has NO idea what this button does. Fix: <button class="p-2" aria-label="Delete item"><TrashIcon /><span class="sr-only">Delete item</span></button>. Also: no focus-visible:ring-2 on the button — keyboard users cannot see which button is focused. Fix: add focus-visible:ring-2 focus-visible:ring-primary/50 to EVERY interactive element. Contrast: text-gray-400 on bg-white = 3.5:1 ratio. WCAG AA requires 4.5:1. Fail. Fix: text-gray-600 on bg-white = 5.7:1. Compliant), and @apply Proliferation (200 lines of @apply defeating Tailwind's purpose — a CSS file: .btn { @apply px-4 py-2 rounded-md font-medium text-white bg-primary hover:bg-primary/90 focus-visible:ring-2 focus-visible:ring-primary/50 transition-colors; } .btn-sm { @apply px-3 py-1.5 text-sm rounded; } .btn-lg { @apply px-6 py-3 text-lg rounded-lg; } ...200 lines of @apply classes. This is just writing CSS with extra steps. The utility-first philosophy is lost. In Tailwind v4: use @utility instead of @apply for custom utilities. Better: use component files (React/Vue/Svelte) to encapsulate repeated patterns. The classes stay in the template. The component IS the abstraction. @apply is acceptable for: base styles on html/body, prose typography, third-party overrides. Everything else: classes in the template, extracted to components when > 10 utilities). Call once per component or page


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tailwind Excellence Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I'll create a pricing card with bg-[#6366f1], text-[#ffffff], w-[380px], mt-[32px], wrapped in divs, no dark mode, desktop only."

**🤖 AI Agent:**
> Verdict: DESIGN_SYSTEM_ABSENT. Define @theme tokens: --color-primary: #6366f1 (then bg-primary), --spacing-8 for mt-8, consistent widths via max-w-sm. Add dark mode (dark:bg-gray-900). Use semantic HTML (section/article). Add responsive breakpoints.

---

**👤 You:**
> "@theme with --color-primary (50-950), --spacing scale, --radius scale. PricingCard: <section> with <article>, focus-visible:ring on CTA, sr-only on icon, dark:bg-gray-900. grid-cols-1 md:grid-cols-2 lg:grid-cols-3. hover:bg-primary/90 transition-colors."

**🤖 AI Agent:**
> Verdict: UI_PROVEN. Design tokens in @theme (color scale, spacing, radius). Semantic HTML (section/article). Accessible (focus-visible, sr-only, dark mode). Mobile-first responsive (grid breakpoints). Clean architecture (hover/transition states). Ship it.

---

**👤 You:**
> "I'll build a nav with @theme tokens, proper colors, but all divs, no <nav> element, no aria-label, no focus states on links, and no responsive — desktop fixed width only."

**🤖 AI Agent:**
> Verdict: ACCESSIBILITY_VIOLATED. Tokens and colors correct, but: use <nav> not <div>, add aria-label='Main navigation', focus-visible:ring-2 on every link, sr-only for screen readers. Semantic HTML + ARIA are non-negotiable.


## ❓ FAQ

**Q: Does it generate Tailwind code?**
No. The agent writes the UI. The tool VALIDATES that it follows design system principles — @theme tokens instead of arbitrary values, semantic HTML for accessibility, mobile-first responsive strategy, and clean component architecture with proper state variants.

**Q: Does it support Tailwind v4?**
Yes. Tailwind v4 awareness is built in: @theme for design tokens (not tailwind.config.js), @import 'tailwindcss' (not @tailwind directives), @utility for custom utilities, @variant for custom variants, built-in container queries, and automatic content detection. It catches v3 anti-patterns in v4 projects.

**Q: Why is accessibility a dedicated pillar?**
Because AI agents consistently generate div soup with no semantic HTML, no focus states, and no ARIA. Tailwind makes styling effortless but semantic structure and accessibility still require deliberate choices. This tool forces: semantic elements, focus-visible:ring, sr-only text, contrast ratios, and motion-safe variants.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tailwind-excellence-prover](https://vinkius.com/mcp/tailwind-excellence-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tailwind Excellence Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tailwind-excellence-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tailwind Excellence Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tailwind-excellence-prover": {
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
