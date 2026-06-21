# Accessibility Prover MCP Server

Accessibility Prover is a pre-build validation system that forces WCAG 2.2 AA compliance before code is written. It audits semantic HTML, keyboard navigation, contrast ratios (4.5:1 minimum), screen reader compatibility, and motion safety across 5 structured Decision Pivots. Unlike runtime scanners, it catches div soup, missing focus traps, and inaccessible animations during the design phase — before they reach production and before they violate the European Accessibility Act (EAA 2025).

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/accessibility-prover)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
Accessibility Prover validates user interface specifications against WCAG 2.2 AA standards using structured reasoning — not DOM scanning. It acts as a pre-build gate that forces AI agents and front-end developers to satisfy accessibility rules before writing component code.

### The Problem It Solves

Five accessibility barriers account for 92% of the issues flagged by the WebAIM Million annual report:

- **Div soup** — Replacing semantic tags (`<header>`, `<nav>`, `<main>`, `<button>`) with nested `<div>` structures, rendering the interface invisible to assistive technology. Screen readers cannot infer the role of a `<div onclick>` — it is functionally absent.
- **Keyboard trapped** — Leaving interactive elements unreachable by keyboard navigation, removing visible focus indicators, or failing to trap focus inside active modals. 2.5 million keyboard-only users in the EU cannot use a button they cannot reach.
- **Contrast failing** — Using color combinations below the WCAG 2.2 AA 4.5:1 minimum ratio (3:1 for large text). A contrast ratio of 2.1:1 means 1 in 12 men with color vision deficiency cannot read the label.
- **Screen reader blind** — Omitting image alt texts, aria-labels on icon buttons, or form-label associations. An unlabeled `<button>` with an SVG icon is announced as "button" with no context — the user does not know what it does.
- **Motion hostile** — Animations without `prefers-reduced-motion` media queries trigger vestibular disorders affecting 35% of adults over 40. Auto-playing carousels and parallax scrolling are the most common offenders.

### How It Works

Accessibility Prover validates UI specifications using 5 Decision Pivots. Each pivot produces one of six structured verdicts: A11Y_PROVEN, DIV_SOUP, KEYBOARD_TRAPPED, CONTRAST_FAILING, SCREEN_READER_BLIND, or MOTION_HOSTILE.

1. **semanticHTML** — Are correct HTML5 elements used for their intended purpose? `<button>` for actions, `<a>` for navigation, `<input>` for form fields. Custom `<div>` or `<span>` elements with click handlers are rejected.
2. **keyboardNavigable** — Is there a logical tab order? Are focus indicators visible (`:focus-visible`)? Do modals and dialogs implement focus traps? Can the user escape every interactive region?
3. **contrastCompliant** — Do foreground/background color combinations satisfy the 4.5:1 ratio across default, hover, focus, active, and disabled states? Large text (18px+ or 14px+ bold) allows 3:1.
4. **screenReaderReady** — Are images described (`alt`), icon buttons labeled (`aria-label`), form fields associated (`<label for>`), and decorative elements hidden (`aria-hidden="true"`)?
5. **motionRespected** — Are animations wrapped in `@media (prefers-reduced-motion: no-preference)`? Do transitions respect duration limits? Is auto-play disabled by default?

### Why It Works

- **Shift-left compliance.** Fixing a contrast ratio during design takes 2 minutes. Fixing it after a production accessibility audit takes 2 sprints — plus the legal review, the backlog reprioritization, and the release cycle.
- **EAA 2025 enforcement.** Since June 2025, the European Accessibility Act applies to all digital products sold in the EU. Non-compliance carries fines up to 5% of annual revenue. Accessibility Prover creates an auditable pre-build record that demonstrates due diligence.
- **AI agent guardrail.** When AI coding agents generate front-end code, they default to div-based layouts with decorative styling. Accessibility Prover intercepts the specification and forces semantic HTML, ARIA attributes, and contrast verification before the code is written.


## Available Tools
- **validate_accessibility**: You must: (1) map LANDMARKS using semantic HTML5 elements — <header>, <nav>, <main>, <article>, <section>, <aside>, <footer>. Never use <div> with click handlers in place of <button>. Never use <a> for actions that do not navigate, (2) specify KEYBOARD navigation — tab order (tabindex="0" for custom elements), focus-visible indicators (ban outline:none), modal focus traps (inert on background), roving tabindex for composite widgets, (3) cite NUMERICAL contrast ratios — 4.5:1 minimum for normal text (<18pt/24px), 3:1 minimum for large text (≥18pt/24px or ≥14pt bold). Include hover/focus state ratios, (4) define SCREEN READER context — descriptive alt texts (not "image of"), aria-label on icon-only buttons, explicit <label for="id"> on form inputs, aria-describedby for validation, aria-live for dynamic content, (5) define MOTION safety — prefers-reduced-motion CSS overrides for all transitions and animations, pause controls on auto-playing media, no content-conveying-only-through-motion. If the tool rejects, your UI design contains accessibility barriers — fix them before building.

Structured reflection tool for accessibility compliance (WCAG 2.2 AA / EAA 2025 / Section 508). Forces the agent to validate semantic HTML landmarks, keyboard navigation specs, text/background contrast ratios, screen reader ARIA annotations, and motion media queries BEFORE building a component. Catches Div Soup (no semantic landmarks), Keyboard Traps (unreachable interactive elements), Contrast Failures (ratios below 4.5:1), Screen Reader Blindness (missing alt/aria-label/form associations), and Motion Hostility (no prefers-reduced-motion). Call once per UI view or complex component


## Installation & Usage

To install and use the **Accessibility Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/accessibility-prover](https://vinkius.com/mcp/accessibility-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
