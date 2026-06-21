# Accessibility Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/accessibility-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Accessibility Prover is a pre-build validation system that forces WCAG 2.2 AA compliance before code is written. It audits semantic HTML, keyboard navigation, contrast ratios (4.5:1 minimum), screen reader compatibility, and motion safety across 5 structured Decision Pivots. Unlike runtime scanners, it catches div soup, missing focus traps, and inaccessible animations during the design phase — before they reach production and before they violate the European Accessibility Act (EAA 2025).

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


## Available Tools (1)
- **validate_accessibility**: You must: (1) map LANDMARKS using semantic HTML5 elements — <header>, <nav>, <main>, <article>, <section>, <aside>, <footer>. Never use <div> with click handlers in place of <button>. Never use <a> for actions that do not navigate, (2) specify KEYBOARD navigation — tab order (tabindex="0" for custom elements), focus-visible indicators (ban outline:none), modal focus traps (inert on background), roving tabindex for composite widgets, (3) cite NUMERICAL contrast ratios — 4.5:1 minimum for normal text (<18pt/24px), 3:1 minimum for large text (≥18pt/24px or ≥14pt bold). Include hover/focus state ratios, (4) define SCREEN READER context — descriptive alt texts (not "image of"), aria-label on icon-only buttons, explicit <label for="id"> on form inputs, aria-describedby for validation, aria-live for dynamic content, (5) define MOTION safety — prefers-reduced-motion CSS overrides for all transitions and animations, pause controls on auto-playing media, no content-conveying-only-through-motion. If the tool rejects, your UI design contains accessibility barriers — fix them before building.

Structured reflection tool for accessibility compliance (WCAG 2.2 AA / EAA 2025 / Section 508). Forces the agent to validate semantic HTML landmarks, keyboard navigation specs, text/background contrast ratios, screen reader ARIA annotations, and motion media queries BEFORE building a component. Catches Div Soup (no semantic landmarks), Keyboard Traps (unreachable interactive elements), Contrast Failures (ratios below 4.5:1), Screen Reader Blindness (missing alt/aria-label/form associations), and Motion Hostility (no prefers-reduced-motion). Call once per UI view or complex component


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessibility Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Let's build a close button. It's a div with a click event and an X icon inside."

**🤖 AI Agent:**
> Verdict: DIV_SOUP.

A `<div>` lacks native keyboard focus, Enter/Space activation, and the implicit 'button' ARIA role. Screen readers announce it as generic text — the user does not know it is interactive.

Fix: Replace `<div onclick>` with `<button aria-label="Close dialog">`. Add `focus-visible` styles for keyboard users. Hide the decorative SVG icon with `aria-hidden="true"` so the screen reader uses the aria-label instead.

---

**👤 You:**
> "Component: CloseButton.
Layout: <button class='p-2' aria-label='Close dialog'><svg aria-hidden='true'>...</svg></button>.
Keyboard: native button, focusable. focus-visible: 2px solid outline.
Contrast: icon is #4A5568 on #FFFFFF background. Ratio: 4.62:1.
Screen Reader: aria-label='Close dialog' on button. SVG hidden.
Motion: no animations."

**🤖 AI Agent:**
> Verdict: A11Y_PROVEN.

✓ semanticHTML — Native `<button>` with correct implicit role.
✓ keyboardNavigable — Focusable by default, visible focus indicator present.
✓ contrastCompliant — 4.62:1 exceeds the 4.5:1 AA minimum for standard text.
✓ screenReaderReady — aria-label provides clear context. Decorative SVG hidden.
✓ motionRespected — No animations present, no motion risk.

---

**👤 You:**
> "Component: CloseButton.
Layout: <button aria-label='Close dialog'><svg>...</svg></button>.
Keyboard: native button.
Contrast: icon color #E2E8F0 on #FFFFFF background. Ratio: 1.28:1.
Screen Reader: aria-label set.
Motion: none."

**🤖 AI Agent:**
> Verdict: CONTRAST_FAILING.

✗ contrastCompliant — Ratio 1.28:1 fails the WCAG 2.2 AA minimum of 4.5:1 by a factor of 3.5×. The icon is effectively invisible to users with low vision or color deficiency.

Fix: Change icon color to #4A5568 (4.62:1) or #374151 (6.33:1) to exceed the 4.5:1 threshold. Verify the ratio in hover and focus states as well — not just default.

---

**👤 You:**
> "Component: NotificationBanner.
Layout: <div role='alert'> with a dismiss button (<span onclick='close()'>×</span>).
Keyboard: dismiss element is not focusable.
Contrast: text #1F2937 on #FEF3C7 background. Ratio: 8.19:1.
Screen Reader: role='alert' is set on the container. Dismiss has no label.
Motion: banner slides in from the top with 300ms ease-in."

**🤖 AI Agent:**
> Verdict: KEYBOARD_TRAPPED + DIV_SOUP.

✓ contrastCompliant — 8.19:1 exceeds the 4.5:1 minimum.
✓ screenReaderReady (partial) — role='alert' is correct for live announcements.
✗ semanticHTML — Dismiss uses `<span onclick>`, which has no keyboard access or ARIA role. Replace with `<button aria-label="Dismiss notification">`.
✗ keyboardNavigable — Dismiss is unreachable by Tab. Keyboard users cannot close the notification.
✗ motionRespected — 300ms slide animation lacks `prefers-reduced-motion` check. Wrap in `@media (prefers-reduced-motion: no-preference)` or provide `transition: none` fallback.


## ❓ FAQ

**Q: Why does Accessibility Prover reject divs with click handlers?**
A `<div>` has no native keyboard interactivity, no focusability, and no implicit ARIA role. Adding `onclick` creates a visual button that keyboard and screen reader users cannot operate. Native `<button>` elements provide focus, Enter/Space activation, and the 'button' role automatically — no extra JavaScript required.

**Q: What is a focus trap and when is it required?**
A focus trap constrains Tab navigation inside a specific element — typically a modal, dialog, or dropdown — so users cannot navigate to the underlying page while the overlay is active. WCAG 2.4.3 (Focus Order) requires it for all modal dialogs. Without it, a keyboard user can Tab behind the modal into invisible content.

**Q: Does Accessibility Prover check contrast across all interactive states?**
Yes. The contrastCompliant pivot validates foreground/background color combinations across five states: default, hover, focus, active, and disabled. A button that passes contrast in its default state but fails on hover (e.g., light gray text on white) is flagged as CONTRAST_FAILING.

**Q: How is this different from axe-core or Lighthouse?**
axe-core and Lighthouse scan rendered HTML in a browser — they detect violations after the code is built and running. Accessibility Prover validates UI specifications before code is written. It reasons about component behavior, keyboard flows, and interaction states at the design level, catching architectural issues that post-build scanners cannot see because they only inspect the final DOM.

**Q: Can I use Accessibility Prover with an AI coding agent?**
Yes — that is a primary use case. AI coding agents default to div-based layouts because divs are syntactically simpler. Accessibility Prover acts as a guardrail: the agent submits its component specification, the prover validates it against 5 pivots, and the agent receives a structured verdict with specific fixes before writing code.

**Q: What does the European Accessibility Act (EAA 2025) mean for my product?**
Since June 2025, the EAA requires all digital products and services sold in the EU to meet accessibility standards equivalent to WCAG 2.1 AA (with WCAG 2.2 AA as the recommended benchmark). Non-compliance carries fines up to 5% of annual revenue and potential market withdrawal. Accessibility Prover helps demonstrate compliance as a build-time gate, creating an auditable validation record.

**Q: What input format does Accessibility Prover expect?**
Submit each component as structured text covering 5 dimensions: (1) Layout — the HTML elements and hierarchy, (2) Keyboard — tab order, focus indicators, focus traps, (3) Contrast — foreground and background hex values with computed ratio, (4) Screen Reader — alt texts, aria-labels, form-label associations, (5) Motion — animation properties and prefers-reduced-motion handling. The tool reasons about each dimension independently.

**Q: Does Accessibility Prover support WCAG 2.2 AAA?**
The tool validates against WCAG 2.2 AA, which is the legally required level under the EAA 2025 and the practical target for most products. AAA requirements (e.g., 7:1 contrast ratio, sign language interpretation) are not enforced — they are aspirational goals that few products achieve fully.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/accessibility-prover](https://vinkius.com/mcp/accessibility-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessibility Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessibility-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessibility Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessibility-prover": {
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
