# Succession Planting Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/succession-planting-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Generate optimized planting schedules for continuous crop harvesting.

## Description
This MCP server provides tools to manage continuous crop harvesting through optimized succession planting. It calculates valid sowing dates based on biological maturity, seasonal constraints, and succession intervals. Use `get_planting_schedule` to map out an entire season, `validate_planting_viability` to check if a specific date is safe, or `calculate_total_yield_potential` to estimate the number of harvests possible. It helps gardeners and farmers ensure a steady food supply by respecting final planting cutoffs and harvest windows.


## Available Tools (4)
- **get_next_planting_gap**: Tells the user how many days they must wait before they can plant again to maintain the succession pattern
- **calculate_total_yield_potential**: Estimates how many successive harvests can be achieved within a single season
- **get_planting_schedule**: Calculates a complete list of all valid planting dates and their corresponding expected harvest dates
- **validate_planting_viability**: Determines if a single specific planting attempt is biologically feasible given the seasonal constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Succession Planting Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a planting schedule starting 2024-03-01, with 30 days maturity, a 14-day succession interval, a cutoff of 2024-07-01, and a harvest end of 2024-08-01."

**🤖 AI Agent:**
> Your planting schedule is: 2024-03-01 (Harvest: 2024-03-31), 2024-03-15 (Harvest: 2024-04-14), 2024-03-29 (Harvest: 2024-04-28), 2024-04-12 (Harvest: 2024-05-12), 2024-04-26 (Harvest: 2024-05-26), 2024-05-10 (Harvest: 2024-06-09), 2024-05-24 (Harvest: 2024-06-23), 2024-06-07 (Harvest: 2024-07-07).

---

**👤 You:**
> "Is it safe to plant on 2024-09-15 if maturity is 40 days, cutoff is 2024-10-01, and harvest end is 2024-11-01?"

**🤖 AI Agent:**
> No, the planting is not viable because the expected harvest date would exceed the harvest window end.

---

**👤 You:**
> "How many days until my next planting if I last planted on 2024-05-01 and my interval is 20 days?"

**🤖 AI Agent:**
> You have 12 days remaining until your next scheduled planting.


## ❓ FAQ

**Q: How do I know if my planting date is safe?**
You can use the `validate_planting_viability` tool to check if a specific date is biologically feasible given your seasonal constraints.

**Q: Can I plan an entire season at once?**
Yes, the `get_planting_schedule` tool generates a complete list of all valid planting and harvest dates for your entire season.

**Q: How many times can I plant the same crop?**
Use the `calculate_total_yield_potential` tool to estimate the total number of successful planting cycles possible within your growing season.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/succession-planting-calendar](https://vinkius.com/en/ai-agent-connect/succession-planting-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Succession Planting Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `succession-planting-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Succession Planting Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "succession-planting-calendar": {
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
