# Family Event Cost Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-event-cost-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track and analyze expenditures for family celebrations and events.

## Description
Manage the financial side of family gatherings with precision. This MCP server allows AI agents to record individual expenses using `add_event_expense`, retrieve comprehensive financial overviews via `get_event_summary`, filter events by theme with `list_events_by_category`, and perform detailed guest-based cost analysis using `calculate_event_per_person_breakdown`.


## Available Tools (4)
- **calculate_event_per_person_breakdown**: Analyze how costs are distributed per guest for a specific event
- **get_event_summary**: Retrieve a high-level financial overview of a specific event
- **list_events_by_category**: Find all events that fall under a specific thematic classification
- **add_event_expense**: Ensure the eventId is correct and amount is positive.

Record a new individual cost item for a specific family event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Event Cost Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Add a $50 expense for catering to event 'birthday-2024'."

**🤖 AI Agent:**
> The expense for catering has been successfully recorded for event 'birthday-2024'.

---

**👤 You:**
> "What is the total cost and budget variance for event 'wedding-01' with a planned budget of $5000?"

**🤖 AI Agent:**
> The total cost for 'wedding-01' is $4500, resulting in a budget variance of $500.

---

**👤 You:**
> "Calculate the cost per person for event 'reunion-2023' with 15 attendees."

**🤖 AI Agent:**
> The cost per person for the 'reunion-2023' event is $33.33.


## ❓ FAQ

**Q: How do I record a new expense?**
You can use the `add_event_expense` tool to record a description, amount, and category for any specific event ID.

**Q: Can I see how much I am over or under my budget?**
Yes, by using `get_event_summary` and providing a planned budget, the tool calculates the budget variance for you.

**Q: How is the cost per person calculated?**
The `calculate_event_per_person_breakdown` tool divides the total accumulated expenses by the number of attendees you provide.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-event-cost-tracker](https://vinkius.com/en/ai-agent-connect/family-event-cost-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Event Cost Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-event-cost-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Event Cost Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-event-cost-tracker": {
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
