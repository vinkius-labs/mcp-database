# UI/UX Excellence Prover MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uiux-excellence-prover)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/uiux-excellence-prover-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/uiux-excellence-prover-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

AI agents generate flat, lifeless interfaces: decorative shadows, linear animations, buttons without hover states, chaotic spacing, and accessibility theater. This tool enforces 2026-era excellence: spatial hierarchy with Liquid Glass, spring-based motion, 8-state microinteractions, 8...

## Description
AI agents produce interfaces that function but fail to reach the quality bar of a senior UI/UX designer working in 2026.

### The Problem

- **Flat decoration** — Shadows and gradients as ornament, not spatial communication
- **Gratuitous motion** — Animation that entertains but doesn't explain, guide, or confirm
- **Dead interactions** — Buttons with no hover, no active press, no loading, no success feedback
- **Rhythm collapse** — Random spacing, inconsistent typography, no grid system
- **Accessibility theater** — Looks compliant but fails keyboard, screen reader, and neurodivergent users
- **Dark patterns** — Infinite scroll, auto-play, fake urgency, hidden controls

### Six Pillars of 2026 Interface Mastery

1. **Spatial Hierarchy** — Elevation 0-5, Liquid Glass materiality, dark mode via surface lightness
2. **Motion System** — Spring physics (stiffness/damping), purpose-only, motion tokens, 60fps
3. **Microinteraction Polish** — 8 states per element (idle/hover/active/focus/disabled/loading/success/error)
4. **Visual Rhythm** — 8px grid, modular typographic scale, macro/micro spacing, optical alignment
5. **Neuro-Inclusive A11y** — WCAG 2.2 AAA, prefers-reduced-motion, low-stimulus mode, progressive disclosure
6. **Agency & Calm UI** — Zero dark patterns, intentional friction, natural stopping points


## Available Tools
- **validate_uiux_excellence**: 1. SPATIAL: Elevation levels 0-5 with semantic meaning. Shadow tokens (not arbitrary box-shadow). Dark mode via surface lightness variation (not color inversion). Liquid Glass for overlays. 2. MOTION: Every animation EXPLAINS, GUIDES, or CONFIRMS. Spring physics (not linear easing). 60fps. Motion tokens (duration, stiffness, damping). `prefers-reduced-motion` fallback. 3. MICRO: 8 states per interactive element (default, hover, focus-visible, active/pressed, loading, success, error, disabled). Touch targets ≥44×44px. Feedback within 100ms. 4. RHYTHM: 8px base grid. Modular typographic scale (3:1+ ratio heading to body). Macro whitespace (24-48px) vs micro (4-8px) — contrast creates hierarchy. 5. A11Y: WCAG 2.2 AAA. aria-label on icon buttons. alt text on images. focus-visible:ring on ALL interactive elements. Contrast ≥4.5:1. prefers-* media queries. Keyboard navigation. Screen reader testing (NVDA/VoiceOver). 6. AGENCY: Zero dark patterns. Nothing pre-checked. Equal visual weight for opt-in/opt-out. Progressive disclosure. Natural stopping points. No auto-play video. No infinite scroll without pause.

Ultra-expert UI/UX validation for 2026-era interfaces — forces spatial hierarchy, motion purpose, microinteraction completeness, visual rhythm, genuine accessibility, and user agency. Based on: Don Norman ("The Design of Everyday Things," 1988 — affordances and feedback), Dieter Rams (10 Principles of Good Design — "less but better"), and Apple Human Interface Guidelines (2024 — Liquid Glass, spatial computing, semantic depth). Catches Flat Decoration (surfaces that look identical — no depth hierarchy communicates affordance — an elevator panel: all 20 buttons the same size, same color, same depth. Which is the "close door" button? Which is the emergency? Which is your floor? The emergency button should be RED, LARGER, physically RAISED, and TEXTURED — findable by touch without looking. The floor buttons should be in a GRID with tactile numbers. The "close door" button should be smaller and recessed — it is secondary. Flat decoration means: "everything is equally important" = "nothing is important." Fix: elevation levels 0-5 with semantic meaning. Level 0: background surface. Level 1: card. Level 2: floating action. Level 3: modal overlay. Level 4: toast notification. Level 5: critical alert. Each level has a distinct shadow, blur, and z-index), Gratuitous Motion (animation that exists for spectacle, not communication — a restaurant menu on a tablet: page loads with a 3-second cascading animation. Every dish card flies in from the left, bounces, rotates 360°, and settles. The customer is hungry. They want to ORDER, not watch a show. The animation adds 3 seconds of delay with zero information value. Purposeful motion: a loading skeleton shows content shape (sets expectation). A transition between pages slides in the direction of navigation (communicates spatial model). A success checkmark draws itself (confirms completion). Every animation must answer: what does this EXPLAIN, GUIDE, or CONFIRM? If the answer is "it looks cool": remove it. Use spring physics for natural feel. 60fps mandatory. `prefers-reduced-motion: reduce` fallback for vestibular sensitivity), Dead Interactions (buttons with only 2 states: default and clicked — a hotel booking button: click it — nothing happens for 2 seconds — page refreshes. Did it work? Was it clicked? Is it processing? Did it fail? The button needed 8 states: default → hover (cursor change + subtle highlight) → focus-visible (keyboard ring) → active/pressed (spring scale-down) → loading (spinner + disabled) → success (checkmark + green) → error (shake + red message) → disabled (grayed out, cursor: not-allowed). 8 states per interactive element is not over-engineering — it is basic communication. Touch targets: minimum 44×44px (WCAG 2.2). Feedback within 100ms of interaction), Rhythm Collapsed (inconsistent spacing and typography creating visual noise — a printed newspaper with 14px body text and 15px headings. The heading is barely distinguishable from the body. There is no hierarchy. The eye does not know where to start or what matters. Fix: modular typographic scale with at least 3:1 ratio between heading and body. Body: 16px. H3: 20px. H2: 28px. H1: 48px. Spacing: 8px base grid. Micro: 4-8px (within components). Macro: 24-48px (between sections). Dramatic: 80-160px (section breathing room). The CONTRAST between tight clusters and generous whitespace IS the rhythm), Accessibility Theater (claiming compliance without genuine inclusion — a museum website: "WCAG 2.2 AA compliant." Screen reader test: "button. button. button. button." 47 unlabeled buttons. No `aria-label`. No alt text on exhibition images. Keyboard navigation: Tab key skips the entire main content and jumps to the footer. Color contrast: 2.8:1 on grey-on-light-grey text (minimum: 4.5:1 for AA). The compliance badge is decoration. The experience for a blind or keyboard-only user is broken. Fix: WCAG 2.2 AAA (not just AA). `aria-label` on every icon button. Alt text on every meaningful image. `focus-visible:ring` on every interactive element. `prefers-color-scheme`, `prefers-reduced-motion`, `prefers-contrast`. Screen reader testing with NVDA/VoiceOver — not just automated Lighthouse), and Dark Pattern Detected (design that tricks users into actions against their interest — a flight booking checkout: a $47 travel insurance option is PRE-CHECKED. The uncheck button is grey text on light grey background (contrast: 1.8:1). The "Continue without insurance" link is below the fold. The "Add insurance" button is green, large, and prominent. This is a "roach motel" + "misdirection" + "sneak into basket" dark pattern. Fix: nothing pre-checked. Equal visual weight for "yes" and "no" options. Clear cost display. Natural stopping points where the user can review what they are buying. Progressive disclosure: show complexity only when the user asks for it). Call once per interface, component, or design review


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UI/UX Excellence Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I'll build a dashboard with cards using box-shadow, CSS ease-in-out animations, buttons with hover color change only, random padding values, and a dark mode toggle."

**🤖 AI Agent:**
> Verdict: FLAT_DECORATION. Shadows are decorative — define elevation 0-5 with semantic roles. Replace ease-in-out with spring physics. Buttons need 8 states (idle/hover/active/focus/disabled/loading/success/error). Standardize to 8px grid. Dark mode needs surface lightness, not just color swap.

---

**👤 You:**
> "KPI cards: elevation 1→2 on hover (spring stiffness 400). Chart: skeleton loading with pulse, error state with retry button. Sidebar: spring slide from right (300ms, damping 20). 8px grid. WCAG 2.2 AAA. prefers-reduced-motion: fade fallback. No infinite scroll — paginated data table."

**🤖 AI Agent:**
> Verdict: DESIGN_PROVEN. Spatial hierarchy (elevation 1→2 with spring). Motion system (spring physics, skeleton loading, reduced-motion fallback). 8-state interactions (loading, error+retry). 8px rhythm. WCAG AAA. Calm UI (paginated, no infinite scroll). Ship it.

---

**👤 You:**
> "I'll add parallax scrolling background, particle effects, auto-playing hero video, infinite scroll feed, and confetti animation on every form submission."

**🤖 AI Agent:**
> Verdict: DARK_PATTERN_DETECTED. Parallax/particles = decorative noise without communicative purpose. Auto-play violates user agency. Infinite scroll is an attention trap (add 'Load more' or pagination). Confetti on every submit = cognitive overload. Every animation must EXPLAIN, GUIDE, or CONFIRM — nothing else.


## Installation & Usage

To install and use the **UI/UX Excellence Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uiux-excellence-prover](https://vinkius.com/mcp/uiux-excellence-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
