# Local Waterfront Visit Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-waterfront-visit-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Validate waterfront visit feasibility, facility access, and logistics.

## Description
This MCP server provides decision-support tools for planning waterfront excursions. It allows AI agents to determine if a visit is viable using `plan_visit_feasibility`, check if specific activities are allowed via `check_facility_access`, calculate precise arrival and departure times with `calculate_logistics_window`, and prepare for weather changes using `generate_contingency_plan`.


## Available Tools (4)
- **calculate_logistics_window**: Maps out the specific arrival and departure timestamps based on the user's duration and planned start
- **check_facility_access**: Validates if specific activities or facilities are accessible to the group based on permits and companion types
- **generate_contingency_plan**: Provides an alternative plan if the primary visit is invalidated by a change in conditions
- **plan_visit_feasibility**: Determines if a visit to a specific waterfront is possible given all user constraints and location rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Waterfront Visit Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is it feasible to visit Pier 37 with 3 companions for 120 minutes by car if it is Sunny?"

**🤖 AI Agent:**
> Yes, the visit to Pier 37 is viable. Your group is approved, and you can use the available walking paths and benches.

---

**👤 You:**
> "Can I go kayaking at the waterfront if I don't have a permit?"

**🤖 AI Agent:**
> No, kayaking requires a specific permit. You will need to obtain the Watercraft Permit before this activity is accessible.

---

**👤 You:**
> "Calculate my arrival and departure if I start at 2024-07-04T10:00:00Z for 90 minutes."

**🤖 AI Agent:**
> You will arrive at 2024-07-04T10:00:00Z and depart at 2024-07-04T11:30:00Z.


## ❓ FAQ

**Q: How do I know if my visit is possible?**
You can use the `plan_visit_feasibility` tool to check if your group, weather conditions, and transportation mode align with the location's rules.

**Q: Can I check if I need a permit for kayaking?**
Yes, the `check_facility_access` tool will tell you if an activity is accessible and if a specific permit is required.

**Q: What happens if the weather changes?**
You can use `generate_contingency_plan` to receive a recommendation, such as an indoor alternative or a rescheduling suggestion, based on the new conditions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-waterfront-visit-planner](https://vinkius.com/en/ai-agent-connect/local-waterfront-visit-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Waterfront Visit Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-waterfront-visit-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Waterfront Visit Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-waterfront-visit-planner": {
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
