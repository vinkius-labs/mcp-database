# Holiday Weekend Bridge Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/holiday-weekend-bridge-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Maximize your long weekends by identifying the most efficient PTO bridge days.

## Description
The Holiday Weekend Bridge Optimizer helps you strategically plan your time off. By analyzing public holidays, it identifies 'bridge' opportunities--Mondays or Fridays that, if taken as PTO, connect a holiday to a weekend for maximum consecutive days off. Using tools like `find_bridge_candidates`, `rank_bridge..' and `optimize_holiday_plan`, you can determine exactly which days to request based on your available PTO budget.


## Available Tools (4)
- **find_bridge_candidates**: Find potential bridge days in a given year
- **calculate_optimization_result**: Calculate the final summary of an optimized plan
- **rank_bridge_candidates**: Rank bridge candidates by efficiency
- **optimize_holiday_plan**: Optimize a holiday plan using available PTO


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Holiday Weekend Bridge Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find potential bridge days for 2025."

**🤖 AI Agent:**
> I found several candidates for 2025, including Monday, May 26th and Friday, July 4th.

---

**👤 You:**
> "Rank these bridge candidates: [{"date": "2025-05-26", "efficiency": 4.0}, {"date": "2025-07-04", "efficiency": 3.0}]"

**🤖 AI Agent:**
> The highest efficiency bridge is May 26th, followed by July 4th.

---

**👤 You:**
> "I have 2 PTO days. What is my best plan using these candidates: [{"date": "2025-05-26", "efficiency": 4.0}, {"date": "2025-07-04", "efficiency": 3.0}]"

**🤖 AI Agent:**
> Your optimal plan is to take off May 26th and July 4th, gaining a total of 7 days off.


## ❓ FAQ

**Q: How does the optimizer find bridge days?**
It uses `find_bridge_candidates` to scan holidays for Tuesdays or Thursdays, identifying the adjacent Mondays or Fridays as potential bridges.

**Q: How is efficiency calculated?**
Efficiency is the ratio of total consecutive days off gained to the number of PTO days used. `rank_bridge_candidates` sorts these for you.

**Q: Can I use my specific PTO budget?**
Yes, by using `optimize_holiday_plan`, you can input your exact available PTO days to get a customized vacation plan.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/holiday-weekend-bridge-optimizer](https://vinkius.com/mcp/holiday-weekend-bridge-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Holiday Weekend Bridge Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `holiday-weekend-bridge-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Holiday Weekend Bridge Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "holiday-weekend-bridge-optimizer": {
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
