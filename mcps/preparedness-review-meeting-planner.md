# Preparedness Review Meeting Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/preparedness-review-meeting-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transforms raw household preparedness data into structured review agendas and actionable execution plans.

## Description
This MCP server acts as an automated coordinator for household emergency readiness. It uses specialized tools to transform raw data--such as household composition, current supply levels, and identified gaps--into a structured meeting agenda. Users can utilize `generate_meeting_agenda` to create discussion guides, `calculate_supply_needs` to estimate procurement costs, and `evaluate_meeting_closure` to ensure all critical gaps are addressed before finalizing a plan. The final output is a formal action plan produced via `create_action_plan`, ensuring every task has an owner and a deadline.


## Available Tools (4)
- **create_action_plan**: Produces the formal output of the meeting, including decisions and next steps
- **generate_meeting_agenda**: Transforms raw preparedness data into a structured discussion guide
- **calculate_supply_needs**: Translates identified gaps into specific procurement requirements based on household size
- **evaluate_meeting_closure**: Determines if the review meeting has met the criteria to finalize the plan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Preparedness Review Meeting Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a meeting agenda for a household with 2 adults and 1 dog, where we are missing water and first aid kits."

**🤖 AI Agent:**
> The meeting agenda will focus on: 1. Reviewing current water levels, 2. Addressing the first aid kit deficiency, and 3. Assigning tasks for procurement.

---

**👤 You:**
> "How much will it cost to fix our gaps for 4 people if we need water and batteries?"

**🤖 AI Agent:**
> The estimated cost for water and batteries for a 4-person household is $45.00.

---

**👤 You:**
> "Can we close the meeting if we haven't assigned a person to buy the water yet?"

**🤖 AI Agent:**
> No, the meeting cannot be closed until every identified gap has a task owner assigned.


## ❓ FAQ

**Q: How does the tool determine if a meeting is ready to close?**
The `evaluate_meeting_closure` tool ensures closure only occurs if all identified gaps have assigned task owners and the budget for replenishment is confirmed.

**Q: Can I use this to calculate how much food I need to buy?**
Yes, the `calculate_supply_needs` tool translates your identified gaps into specific procurement requirements and estimates the total cost.

**Q: What information is required to generate an agenda?**
To use `generate_meeting_agenda`, you need to provide the current plan, a list of household members, the current supply status, and any identified gaps.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/preparedness-review-meeting-planner](https://vinkius.com/en/ai-agent-connect/preparedness-review-meeting-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Preparedness Review Meeting Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `preparedness-review-meeting-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Preparedness Review Meeting Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "preparedness-review-meeting-planner": {
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
