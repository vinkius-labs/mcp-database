# Color Contrast Checker MCP Server

Instantly verify if your text is readable on any background. WCAG 2.1 AA/AAA compliance in one call — the AI guesses ratios, this engine calculates them.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/color-contrast-checker-alternative)

## Overview
**Category:** developer-tools
**Tools Count:** 1

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


## Installation & Usage

To install and use the **Color Contrast Checker** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/color-contrast-checker-alternative](https://vinkius.com/mcp/color-contrast-checker-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
