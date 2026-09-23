# Curtain Panel Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/curtain-panel-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Calculate the exact number of curtain panels needed for any window.

## Description
This MCP server provides precise tools for window treatment planning. Use `get_required_panel_count` to determine how many panels to purchase based on window width, panel width, and desired fullness. You can also use `validate_fabric_coverage` to check if your selected panels meet your aesthetic goals, `calculate_total_fabric_width` for fabric requirements, or `estimate_curtain_cost` to budget for your project.


## Available Tools (4)
- **calculate_total_fabric_width**: Determines the total amount of fabric width required to meet a specific aesthetic goal
- **estimate_curtain_cost**: Provides a rough cost estimate based on the number of panels needed
- **get_required_panel_count**: Determines exactly how many curtain panels a user needs to purchase for a specific window setup
- **validate_fabric_coverage**: Checks if a specific number of panels provided by a user will provide enough coverage and fullness for their window


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Curtain Panel Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many 50-inch panels do I need for a 100-inch window with double fullness?"

**🤖 AI Agent:**
> You will need 4 panels.

---

**👤 You:**
> "Will 3 panels of 40 inches each be enough for a 60-inch window if I want a fullness of 2.0?"

**🤖 AI Agent:**
> Yes, 3 panels will provide a fullness of 2.0, which meets your requirement.

---

**👤 You:**
> "What is the total fabric width needed for a 72-inch window with a fullness of 2.5?"

**🤖 AI Agent:**
> The total fabric width required is 180 inches.


## ❓ FAQ

**Q: How do I know how many panels to buy?**
You can use the `get_required_panel_count` tool. Simply provide the window width, the width of a single panel, and your desired fullness factor.

**Q: What is a fullness factor?**
The fullness factor is a multiplier that determines how much extra fabric is used to create folds. A factor of 2.0 is standard for decorative pleats.

**Q: Can I estimate the total cost of my curtains?**
Yes, the `estimate_curtain_cost` tool allows you to input the price per panel to get a total estimated cost for your window setup.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/curtain-panel-calculator](https://vinkius.com/en/ai-agent-connect/curtain-panel-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Curtain Panel Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `curtain-panel-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Curtain Panel Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "curtain-panel-calculator": {
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
