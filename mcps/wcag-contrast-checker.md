# WCAG Contrast Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wcag-contrast-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [web-development](../categories/web-development.md)

Evaluate color contrast compliance against WCAG 2.1 and WCAG 3.0 (APCA) standards.

## Description
This MCP server provides essential tools for web accessibility testing by calculating color contrast ratios according to WCAG 2.1 and the newer APCA (WCAG 3.0) models. Use `calculate_contrast` to check specific color pairs, `find_compliant_suggestion` to automatically adjust colors to meet target levels like AA or AAA, and `audit_palette` to validate entire color schemes at once.


## Available Tools (3)
- **audit_palette**: Validates a collection of colors to ensure they all satisfy a specific accessibility standard
- **calculate_contrast**: 1 and APCA results.

Determines the exact contrast ratio and accessibility pass/fail status for two specific colors
- **find_compliant_suggestion**: Suggests a new background color that meets a specific accessibility target by minimally adjusting the current color's lightness


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WCAG Contrast Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the contrast ratio between #FFFFFF and #000000?"

**🤖 AI Agent:**
> The contrast ratio is 21:1, which passes all WCAG 2.1 levels (AA and AAA) and has a high APCA score.

---

**👤 You:**
> "Check if #767676 on #FFFFFF passes WCAG 2.1 AA Normal."

**🤖 AI Agent:**
> The contrast ratio is 4.54:1. It passes the AA Normal and AA Large thresholds, but fails AAA Normal.

---

**👤 You:**
> "Suggest a background color for #FF0000 to meet the AAA_NORMAL standard."

**🤖 AI Agent:**
> The suggested background color is #FFFFFF, which achieves a contrast ratio of 21:1.


## ❓ FAQ

**Q: What standards does this tool support?**
The tool supports WCAG 2.1 (Contrast Ratio) and WCAG 3.0 (APCA - Advanced Perceptual Contrast Algorithm).

**Q: How can I find a color that passes AA standards?**
You can use the `find_compliant_suggestion` tool. Provide your current color and specify 'AA_NORMAL' as the target level.

**Q: Can I check multiple colors at once?**
Yes, use the `audit_palette` tool by providing a JSON array of foreground colors and a single background color.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wcag-contrast-checker](https://vinkius.com/mcp/wcag-contrast-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WCAG Contrast Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wcag-contrast-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WCAG Contrast Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wcag-contrast-checker": {
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
