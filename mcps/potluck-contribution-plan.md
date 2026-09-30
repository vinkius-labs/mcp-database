# Potluck Contribution Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/potluck-contribution-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Coordinate potluck events by matching attendee budgets and dietary needs with food and equipment.

## Description
This MCP server acts as a coordination engine for organizing potluck events. It helps organizers and attendees balance food categories, manage individual budgets, and ensure dietary safety. Use `get_event_summary` to check the readiness of your event, `suggest_contributions` to find items that fit an attendee's profile, `assign_dish` to finalize food contributions, and `manage_equipment` to track necessary serving items like platters or spoons.


## Available Tools (4)
- **assign_dish**: Finalizes a specific food or drink item to an attendee
- **get_event_summary**: Provides a high-level overview of the potluck's current state of readiness
- **manage_equipment**: Tracks and assigns necessary serving equipment to attendees
- **suggest_contributions**: Recommends specific food or drink items to attendees based on their profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Potluck Contribution Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current status of my potluck event with ID event_123?"

**🤖 AI Agent:**
> The event has 12 attendees, the food balance is currently lacking desserts, the total budget allocated is $150, and there is an equipment shortfall of 2 items.

---

**👤 You:**
> "What should attendee_456 bring to the event event_123?"

**🤖 AI Agent:**
> Based on your budget and dietary needs, you could bring a Fruit Salad (category: side, estimated cost: $15) or Veggie Wraps (category: main, estimated cost: $20).

---

**👤 You:**
> "Assign a bowl of potato salad as a side for attendee_789 in event_123 costing $10."

**🤖 AI Agent:**
> The potato salad has been successfully assigned. The new cumulative cost for the event is $110.


## ❓ FAQ

**Q: How can I see if my potluck is ready?**
You can use the `get_event_summary` tool to view the total attendees, food balance, budget status, and any equipment shortfalls.

**Q: How does the system handle dietary restrictions?**
The system ensures dietary safety by using `suggest_contributions` to recommend items that do not conflict with an attendee's profile and validating assignments to prevent dietary violations.

**Q: Can I manage serving spoons and plates through this tool?**
Yes, the `manage_equipment` tool allows attendees to mark items like serving spoons or warming trays as available for the event.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/potluck-contribution-plan](https://vinkius.com/en/ai-agent-connect/potluck-contribution-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Potluck Contribution Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `potluck-contribution-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Potluck Contribution Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "potluck-contribution-plan": {
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
