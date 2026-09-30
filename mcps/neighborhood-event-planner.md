# Neighborhood Event Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/neighborhood-event-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Coordinate community events by managing supplies, volunteers, permits, and schedules.

## Description
This MCP server provides a complete toolkit for organizing community gatherings. It allows AI agents to manage the entire lifecycle of an event, from initial setup to final cleanup. Use `get_event_summary` to monitor budget health and resource counts, `manage_supplies` to track necessary items and costs, and `coordinate_volunteers` to assign personnel to specific roles. You can also use `check_permits_and_compliance` to ensure legal readiness and `plan_activity_schedule` to organize the timeline for setup, execution, or cleanup phases.


## Available Tools (5)
- **check_permits_and_compliance**: Determines if the event is legally cleared to proceed
- **coordinate_volunteers**: Answers questions about personnel availability and task assignments
- **get_event_summary**: Provides a high-level overview of the event's current status and health
- **manage_supplies**: Answers questions regarding what items are needed and how much they cost
- **plan_activity_schedule**: Answers questions about the timeline and the resources required for specific event segments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Neighborhood Event Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current status of event ID 123?"

**🤖 AI Agent:**
> The event is currently on-track with a total budget of $500, $200 spent, 15 volunteers assigned, and 10 supply items listed.

---

**👤 You:**
> "How much will the chairs cost for event 456?"

**🤖 AI Agent:**
> The chairs for event 456 have a total cost of $150 for 10 units.

---

**👤 You:**
> "What activities are planned for the cleanup phase of event 789?"

**🤖 AI Agent:**
> The cleanup phase includes waste removal starting at 4:00 PM and site restoration starting at 5:00 PM.


## ❓ FAQ

**Q: How can I check if my event budget is exceeded?**
You can use the `get_event_summary` tool to view the current status of your event, which will indicate if the budget is over.

**Q: Can I see which volunteers are assigned to setup?**
Yes, by using `coordinate_volunteers` and specifying the 'setup' role, you can see the list of available personnel.

**Q: How do I know if we have the necessary permits?**
Use the `check_permits_and_compliance` tool to compare the required permits against those already acquired.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/neighborhood-event-planner](https://vinkius.com/en/ai-agent-connect/neighborhood-event-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Neighborhood Event Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `neighborhood-event-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Neighborhood Event Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "neighborhood-event-planner": {
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
