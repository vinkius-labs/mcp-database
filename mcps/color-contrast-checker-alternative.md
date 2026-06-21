# Color Contrast Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/color-contrast-checker-alternative)
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


## Available Tools (1)
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


## ❓ FAQ

**Q: My AI says this color combination passes WCAG. Should I trust it?**
No. LLMs cannot reliably calculate relative luminance — they approximate. This engine uses the exact W3C formula: L = 0.2126*R + 0.7152*G + 0.0722*B with sRGB gamma correction. Trust the math, not the prediction.

**Q: What's the difference between AA and AAA levels?**
AA requires 4.5:1 contrast for normal text — the legal minimum in most countries. AAA requires 7:1 — the gold standard for maximum readability. Large text (18pt+) has relaxed thresholds: 3:1 for AA, 4.5:1 for AAA.

**Q: Can I mix color formats? Like HEX for foreground and a CSS name for background?**
Absolutely. Pass '#333333' as foreground and 'white' as background, or 'rgb(0,0,0)' with 'hsl(0,0%,95%)' — the engine normalizes everything internally.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/color-contrast-checker-alternative](https://vinkius.com/mcp/color-contrast-checker-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Color Contrast Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `color-contrast-checker-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Color Contrast Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "color-contrast-checker-alternative": {
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
