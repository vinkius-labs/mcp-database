# Calligraphy Guide Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/calligraphy-guide-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate precise, deterministic calligraphy guide sheets with exact spacing and slant lines.

## Description
This MCP server provides precise geometric calculations for calligraphy practitioners. It allows AI agents to generate exact guide line spacing, including ascender height, descender depth, and baseline positions, based on specific script types like Copperplate, Spencerian, Italic, Gothic, or Modern Brush. By using `generate_guide_dimensions`, you can determine precise vertical and horizontal measurements. You can also use `generate_slant_grid` to calculate the exact placement of diagonal slant lines, and `get_nib_profiles` to identify supported pen widths for accurate spacing logic.


## Available Tools (3)
- **generate_slant_grid**: Determines the positioning and frequency of diagonal slant lines
- **generate_guide_dimensions**: Calculates the exact vertical and horizontal measurements for a single line of calligraphy based on script and x-height
- **get_nib_profiles**: Provides a list of standard available nib widths for calculation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Calligraphy Guide Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the guide dimensions for a Copperplate script with an x-height of 5mm and a 1.0mm nib width."

**🤖 AI Agent:**
> For a Copperplate script with a 5mm x-height and 1.0mm nib, the ascender height is 15mm, the descender depth is 10mm, and the total line height is 30mm.

---

**👤 You:**
> "What are the available nib widths for my calculations?"

**🤖 AI Agent:**
> The available nib widths are 0.3mm, 0.5mm, 1.0mm, 1.5mm, and 2.0mm.

---

**👤 You:**
> "Determine the slant line positions for a 55 degree slant on a 200mm tall page."

**🤖 AI Agent:**
> The slant lines will be placed at 5mm vertical intervals throughout the 200mm page height at a 55 degree angle.


## ❓ FAQ

**Q: How do I calculate spacing for a specific script?**
You can use the `generate_guide_dimensions` tool by providing the script type, the desired x-height in millimeters, and the nib width.

**Q: Can I generate slant lines for my guide sheet?**
Yes, the `generate_slant_grid` tool calculates the exact positioning and frequency of diagonal slant lines based on your specified angle and page height.

**Q: What nib widths are supported?**
You can check all supported widths by calling `get_nib_profiles`. Standard widths include 0.3mm, 0.5mm, 1.0mm, 1.5mm, and 2.0mm.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/calligraphy-guide-calculator](https://vinkius.com/ai-agent-connect/calligraphy-guide-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Calligraphy Guide Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `calligraphy-guide-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Calligraphy Guide Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "calligraphy-guide-calculator": {
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
