# Color Contrast Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/color-contrast-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Check WCAG color contrast compliance via AI — verify text readability against backgrounds for accessible, inclusive web design.

## Description
Connect **Color Contrast Checker** to your AI agent and validate WCAG accessibility compliance for any color combination.

### What you can do

- **Custom Contrast Checks** — Test any foreground/background color pair against WCAG AA and AAA standards
- **Preset Scenarios** — Quickly check text on white, text on black, white text on colors, and black text on colors
- **Dark Mode Validation** — Verify color contrast for dark mode UI designs
- **Light Mode Validation** — Ensure readability in light theme interfaces
- **Accessibility Reporting** — Get instant pass/fail reports with contrast ratios

### How it works

1. Subscribe to this server
2. Enter your Apify API key
3. Start checking color contrast from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **UI/UX Designers** — validate design system colors meet accessibility requirements
- **Web Developers** — check contrast ratios during development without leaving the editor
- **Accessibility Auditors** — batch-verify color compliance across design tokens


## Available Tools (8)
- **check_black_text_on_bg**: Check contrast of pure black text against a specific background
- **check_color_contrast**: 1 contrast ratio for a specific foreground and background color pair to audit visual accessibility.

Check the WCAG contrast ratio between a foreground and background color
- **check_danger_text_contrast**: Check contrast of standard danger/error red text on a background
- **check_dark_mode_surface**: Check contrast against a standard dark mode surface
- **check_light_mode_surface**: Check contrast against a standard light mode surface
- **check_text_on_pure_black**: Check contrast of a text color against a pure black background
- **check_text_on_pure_white**: Check contrast of a text color against a pure white background
- **check_white_text_on_bg**: Check contrast of pure white text against a specific background


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Color Contrast Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if #3B82F6 works on a white background for body text."

**🤖 AI Agent:**
> Contrast ratio: 4.0:1. ❌ Fails WCAG AA for normal text (needs 4.5:1). ✅ Passes WCAG AA for large text (needs 3:1). Consider darkening to #2563EB (contrast 5.4:1) for full AA compliance.


## ❓ FAQ

**Q: What accessibility standards does it check?**
It checks against both WCAG 2.1 Level AA (minimum 4.5:1 for normal text, 3:1 for large text) and Level AAA (7:1 for normal text, 4.5:1 for large text).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/color-contrast-checker](https://vinkius.com/mcp/color-contrast-checker)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `color-contrast-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Color Contrast Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "color-contrast-checker": {
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
