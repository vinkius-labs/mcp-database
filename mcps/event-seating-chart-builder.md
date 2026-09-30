# Event Seating Chart Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/event-seating-chart-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [event-management](../categories/event-management.md)

Optimizes guest seating based on social groups, capacity, and accessibility.

## Description
This MCP server provides a sophisticated engine for managing event seating. It uses `generate_seating_plan` to calculate optimal arrangements that respect guest capacity, social group cohesion, and interpersonal preferences like affinity or separation. It also includes `validate_constraints` to audit existing plans for rule violations, `get_table_proximity_map` to understand spatial relationships between tables, and `check_group_cohesion` to measure how well social groups are preserved.


## Available Tools (4)
- **check_group_cohesion**: Measures how well a seating plan preserves social groups
- **generate_seating_plan**: Calculates an optimized seating arrangement that satisfies all guest constraints and table capacities
- **get_table_proximity_map**: Evaluates the spatial relationship between tables to assist in placement logic
- **validate_constraints**: Audits an existing seating plan to check for violations of rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Event Seating Chart Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a seating plan for 10 guests and 3 tables where Table 1 has a capacity of 4 and Table 2 has a capacity of 4."

**🤖 AI Agent:**
> The seating plan has been generated: Table 1 contains guests A, B, C, and D; Table 2 contains guests E, F, G, and H; Table 3 contains guests I and J.

---

**👤 You:**
> "Check if this seating plan is valid: Guest 1 and Guest 2 are in a separation list but are both assigned to Table 5."

**🤖 AI Agent:**
> The seating plan is invalid. Violation: Guest 1 and Guest 2 cannot be seated at the same table due to separation constraints.

---

**👤 You:**
> "What is the proximity of Table 1 to other tables?"

**🤖 AI Agent:**
> Table 1 is adjacent to Table 2 and Table 3.


## ❓ FAQ

**Q: How does the engine handle guest separation?**
The engine treats separation rules as hard constraints. Using `validate_constraints`, the system ensures that guests marked for separation are never assigned to the same table.

**Q: Can I ensure guests with accessibility needs are accommodated?**
Yes. When using `generate_seating_plan`, the engine matches guest accessibility requirements against available table features to ensure proper placement.

**Q: How can I check if my seating plan is successful?**
You can use `check_group_cohesion` to get a percentage score of how well social groups were kept together, or `validate_constraints` to check for any rule violations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/event-seating-chart-builder](https://vinkius.com/en/ai-agent-connect/event-seating-chart-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Event Seating Chart Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `event-seating-chart-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Event Seating Chart Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "event-seating-chart-builder": {
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
