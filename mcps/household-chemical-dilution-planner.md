# Household Chemical Dilution Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-chemical-dilution-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Calculate precise concentrate and water volumes for cleaning tasks.

## Description
This MCP server provides tools to manage the logistics of preparing cleaning solutions. It calculates the exact amount of concentrate and water needed for specific cleaning tasks based on dilution ratios, task counts, and available inventory. Use `get_required_volumes` to determine mixing needs, `check_inventory_sufficiency` to verify stock, `calculate_bottle_requirements` to plan purchases, and `get_task_summary` for a high-level overview of dilution requirements.


## Available Tools (4)
- **check_inventory_sufficiency**: Verifies if the currently available chemical concentrate is enough to complete the planned dilutions
- **get_required_volumes**: Determines how much fresh concentrate and water must be mixed to satisfy a set of cleaning tasks
- **get_task_summary**: Provides a high-level overview of the dilution requirements for a specific task profile
- **calculate_bottle_requirements**: Determines how many full bottles of concentrate must be purchased or opened to meet the required amount


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Chemical Dilution Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to perform 5 cleaning tasks, each requiring 2 liters of solution with a 1:10 dilution ratio. How much concentrate and water do I need?"

**🤖 AI Agent:**
> You need 0.91 liters of concentrate and 9.09 liters of water to complete the 5 tasks.

---

**👤 You:**
> "I need 5 liters of solution at a 1:5 ratio. I already have 1 liter of solution ready. How much more do I need to mix?"

**🤖 AI Agent:**
> You need to mix 0.67 liters of concentrate and 3.33 liters of water to reach the required volume.

---

**👤 You:**
> "I need 10 liters of concentrate and my bottles are 2.5 liters each. How many bottles should I open?"

**🤖 AI Agent:**
> You need to open 4 bottles.


## ❓ FAQ

**Q: How do I know if I have enough concentrate?**
You can use the `check_inventory_sufficiency` tool by providing the required concentrate amount and your current available stock.

**Q: Can I account for solution I already have prepared?**
Yes, the `get_required_volumes` tool includes an optional parameter for existing solution volume to offset new dilution needs.

**Q: How many bottles do I need to buy?**
The `calculate_bottle_requirements` tool calculates exactly how many full bottles are needed based on the required concentrate and the volume of a single bottle.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-chemical-dilution-planner](https://vinkius.com/en/ai-agent-connect/household-chemical-dilution-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Chemical Dilution Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-chemical-dilution-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Chemical Dilution Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-chemical-dilution-planner": {
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
