# Color Contrast Checker MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/color-contrast-checker-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/color-contrast-checker-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/color-contrast-checker-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Instantly verify if your text is readable on any background. WCAG 2.1 AA/AAA compliance in one call — the AI guesses ratios, this engine calculates them.

## Description
Your agent just picked `#6c757d` text on a `#e9ecef` background. Looks fine, right? Wrong — it fails WCAG AA with a 3.9:1 ratio. Your users with low vision can't read it, and your client's accessibility audit just failed.

This MCP uses the official WCAG 2.1 relative luminance formula to calculate the exact contrast ratio between any two colors. No approximation. No hallucination. Just the math that the W3C defined.

### The Superpowers

- **Full WCAG 2.1 Matrix:** AA and AAA compliance checked for both normal text (4.5:1 / 7:1) and large text (3:1 / 4.5:1) simultaneously.
- **Any Color Format:** Pass HEX, RGB, HSL, or CSS named colors — mix and match freely.
- **Human Verdict:** Returns 'Excellent (AAA)', 'Good (AA)', 'Large Text Only', or 'Fail' — no ratio tables to memorize.
- **Exact Ratio:** The precise contrast ratio to 2 decimal places, not a guess.


## Available Tools
- **check_color_contrast**: Pass foreground and background colors in any format (HEX, RGB, HSL, CSS name). Returns the exact contrast ratio, WCAG AA/AAA pass/fail for both normal and large text, and a human-readable verdict. AI cannot reliably calculate contrast ratios — this engine uses the official WCAG 2.1 relative luminance formula.

Checks WCAG 2.1 color contrast ratio between foreground and background. Returns AA/AAA compliance for normal and large text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Color Contrast Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I'm using white text (#ffffff) on this blue button (#2563eb). Does it pass accessibility standards?"

**🤖 AI Agent:**
> Contrast: 4.68:1 | AA Normal: ✅ Pass | AA Large: ✅ Pass | AAA Normal: ❌ Fail | Verdict: Good (AA)

---

**👤 You:**
> "Our legal team says our website must meet AAA. Check if #1a1a2e background with #e2e8f0 text qualifies."

**🤖 AI Agent:**
> Contrast: 13.2:1 | AAA Normal: ✅ Pass | Verdict: Excellent (AAA) — exceeds all requirements.

---

**👤 You:**
> "The designer wants 'gray' text on a 'lightgray' background for subtle labels. Will users be able to read it?"

**🤖 AI Agent:**
> Contrast: 1.67:1 | Verdict: ❌ Fail — unreadable. Minimum for any text is 3:1. Suggest using #525252 instead.


## Installation & Usage

To install and use the **Color Contrast Checker** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/color-contrast-checker-alternative](https://vinkius.com/mcp/color-contrast-checker-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
