# Paper Craft Sheet Yield MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/paper-craft-sheet-yield)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate paper sheet requirements and layout density for printing jobs.

## Description
This MCP server provides precise calculations for paper manufacturing and printing workflows. It allows AI agents to determine how many templates fit on a master sheet and the total number of sheets required for a specific job. Use `calculate_sheet_yield` to find total sheet counts and layout density, `compare_orientations` to optimize template placement, `validate_margin_constraints` to ensure physical feasibility, and `get_yield_efficiency` to measure material utilization.


## Available Tools (4)
- **compare_orientations**: Compares standard and rotated orientations to find the most efficient layout
- **get_yield_efficiency**: Determines the percentage of the master sheet being utilized by the templates
- **calculate_sheet_yield**: Calculates how many templates fit on one sheet and how many total sheets are needed
- **validate_margin_constraints**: Ensures that the requested margins do not exceed the physical limits of the master sheet


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paper Craft Sheet Yield** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many 5x7 inch templates can I fit on a 25x35 inch sheet with 0.5 inch margins, and how many sheets do I need for 100 copies?"

**🤖 AI Agent:**
> You can fit 24 templates per sheet. For 100 copies, you will need 5 total sheets.

---

**👤 You:**
> "Is it better to rotate a 10x20 template on a 50x50 sheet?"

**🤖 AI Agent:**
> The standard orientation allows for 10 templates, while the rotated orientation allows for 12 templates. Rotating is the better option.

---

**👤 You:**
> "What is the efficiency of fitting 10 templates of 4x4 on a 12x12 sheet?"

**🤖 AI Agent:**
> The utilization is 11.11% and the wasted area is 88.89%.


## ❓ FAQ

**Q: How do I find the best way to arrange my templates?**
You can use the `compare_orientations` tool to compare standard and rotated layouts to find the most efficient fit.

**Q: Can I account for paper waste in my calculations?**
Yes, the `calculate_sheet_yield` tool includes a `wasteRate` parameter to account for unavoidable material loss.

**Q: How does the tool handle margins?**
The tool applies margins to all sides of the sheet. You can use `validate_margin_constraints` to ensure your requested margins are physically possible for your sheet size.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/paper-craft-sheet-yield](https://vinkius.com/en/ai-agent-connect/paper-craft-sheet-yield)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paper Craft Sheet Yield** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paper-craft-sheet-yield` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paper Craft Sheet Yield** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paper-craft-sheet-yield": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
