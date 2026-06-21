# Tailwind Excellence Prover MCP Server

AI agents build bloated styling layers containing arbitrary values, div-only layouts, inaccessible contrast, and legacy configurations. This prover enforces strict design token structures (@theme), utility-first compliance, semantic HTML, mobile-first layouts, and interactive focus states.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tailwind-excellence-prover)

## Overview
**Category:** productivity
**Tools Count:** 1

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


## Available Tools
- **validate_tailwind_excellence**: PILLAR I — DESIGN SYSTEM: Tailwind v4 uses @theme in CSS (NOT tailwind.config.js). Define tokens: --color-primary/secondary/danger (50-950 scale), --spacing-* (4px base), --font-heading/body, --radius-sm/md/lg. Dark mode via dark: variant or color-scheme. NEVER abuse arbitrary values ([347px], [#e74c3c]) — if used >1x it belongs in @theme. PILLAR II — ACCESSIBILITY: semantic HTML (header/main/nav/section, NOT div soup), aria-label on icon buttons, alt on images, sr-only for screen readers, focus-visible:ring-2 on EVERY interactive element, 4.5:1 contrast ratio, motion-safe:/motion-reduce: for animations. PILLAR III — RESPONSIVE: Mobile-first (base=mobile, sm:/md:/lg: upward). Grid: grid-cols-1 md:grid-cols-2 lg:grid-cols-3. @container for component-level responsive. Fluid typography. Touch targets ≥44px. TAILWIND v4: @import "tailwindcss" (no @tailwind directives), @theme for tokens, @utility for custom utilities, @variant for custom variants, automatic content detection. If rejected, fix the design violation.

Structured reflection for Tailwind CSS v4 excellence — forces systematic validation across three pillars: design system integrity, accessibility compliance, and responsive mastery. Built from Tailwind v4 architecture (@import "tailwindcss", @theme block, @utility, @variant, automatic content detection — NOT the legacy tailwind.config.js approach). Catches Arbitrary Value Abuse (using [#e74c3c] and [347px] instead of design tokens — a component uses bg-[#e74c3c] for error states. Searched the codebase: appears 14 times. Another component uses text-[#e74c3c]. A third uses border-[#e74c3c]. 14 occurrences of a hardcoded hex value. If the brand color changes: 14 places to update. One is missed. Now the error state is #e74c3c in 13 places and #e74c4c (typo) in 1 place. Fix: @theme { --color-danger: #e74c3c; } then bg-danger, text-danger, border-danger everywhere. 1 place to update. 0 risk of inconsistency. Rule: if an arbitrary value appears more than once, it belongs in @theme. Acceptable arbitrary use: one-off alignment like top-[3px] that is truly unique), Div Soup (47 nested <div> elements, zero semantic HTML — a pricing page: <div> for header, <div> for nav, <div> for main, <div> for cards, <div> for card content, <div> for footer. 47 divs total. Screen reader announces: "group, group, group, group, group..." — meaningless. Google cannot determine content structure — no article, no section, no heading hierarchy. Fix: <header> for page header, <nav> for navigation, <main> for primary content, <section> for pricing tiers, <article> for each plan, <footer> for page footer. Same Tailwind classes. Completely different semantic meaning. Screen reader: "banner, navigation, main, region: pricing, article: Pro Plan, contentinfo." Semantic HTML costs zero effort — it is choosing the RIGHT element instead of the wrong one), Desktop-First Responsive (writing base styles for desktop and overriding downward — component: grid-cols-3 sm:grid-cols-1. Problem: sm: means "640px and UP" in Tailwind. This is NOT "make it 1 column on mobile." This says: "3 columns at all sizes, then 1 column at 640px+" — the OPPOSITE of intent. On mobile (< 640px): 3 columns. Completely broken layout. Horizontal scroll. Unusable. Fix: grid-cols-1 md:grid-cols-2 lg:grid-cols-3. Base = mobile (1 column). md: = tablet (2 columns). lg: = desktop (3 columns). Mobile-first means: base styles ARE mobile. Breakpoints ADD complexity upward. If you write grid-cols-3 FIRST: you are thinking desktop-first — and mobile is broken), Accessibility Theater (icon-only buttons without aria-label, missing focus states — a delete button: <button class="p-2"><TrashIcon /></button>. Visually: a trash icon. Clear to sighted users. Screen reader: "button." That is all. No label. The user has NO idea what this button does. Fix: <button class="p-2" aria-label="Delete item"><TrashIcon /><span class="sr-only">Delete item</span></button>. Also: no focus-visible:ring-2 on the button — keyboard users cannot see which button is focused. Fix: add focus-visible:ring-2 focus-visible:ring-primary/50 to EVERY interactive element. Contrast: text-gray-400 on bg-white = 3.5:1 ratio. WCAG AA requires 4.5:1. Fail. Fix: text-gray-600 on bg-white = 5.7:1. Compliant), and @apply Proliferation (200 lines of @apply defeating Tailwind's purpose — a CSS file: .btn { @apply px-4 py-2 rounded-md font-medium text-white bg-primary hover:bg-primary/90 focus-visible:ring-2 focus-visible:ring-primary/50 transition-colors; } .btn-sm { @apply px-3 py-1.5 text-sm rounded; } .btn-lg { @apply px-6 py-3 text-lg rounded-lg; } ...200 lines of @apply classes. This is just writing CSS with extra steps. The utility-first philosophy is lost. In Tailwind v4: use @utility instead of @apply for custom utilities. Better: use component files (React/Vue/Svelte) to encapsulate repeated patterns. The classes stay in the template. The component IS the abstraction. @apply is acceptable for: base styles on html/body, prose typography, third-party overrides. Everything else: classes in the template, extracted to components when > 10 utilities). Call once per component or page


## Installation & Usage

To install and use the **Tailwind Excellence Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tailwind-excellence-prover](https://vinkius.com/mcp/tailwind-excellence-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
