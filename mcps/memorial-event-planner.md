# Memorial Event Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/memorial-event-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Coordinate logistics, finances, and timelines for memorial services.

## Description
This MCP server provides a complete coordination suite for organizing memorial services. It allows AI agents to manage venue bookings, catering, floral arrangements, and travel via `manage_logistics_item`. Users can track the entire event status with `get_event_overview`, manage timelines with `get_event_timeline`, split costs among contributors using `calculate_shared_expenses`, and record memorial funds with `track_donations`.


## Available Tools (5)
- **get_event_overview**: 
- **manage_logistics_item**: 
- **get_event_timeline**: 
- **track_donations**: 
- **calculate_shared_expenses**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Memorial Event Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current status of my memorial event?"

**🤖 AI Agent:**
> The event is currently 40% complete. The total estimated budget is $5,000, and $2,000 has been spent so far.

---

**👤 You:**
> "Help me split a $1,200 catering bill between Alice, Bob, and Charlie."

**🤖 AI Agent:**
> Each participant (Alice, Bob, and Charlie) is responsible for $400.

---

**👤 You:**
> "Show me the upcoming tasks for the memorial service."

**🤖 AI Agent:**
> The next tasks are: 1. Confirm floral delivery (Scheduled for tomorrow), 2. Finalize venue payment (Scheduled for Friday).


## ❓ FAQ

**Q: How can I see the total budget for my event?**
You can use the `get_event_overview` tool to see a summary of the total estimated budget and actual spent amounts.

**Q: Can I split the costs between family members?**
Yes, the `calculate_shared_expenses` tool calculates how much each participant is responsible for based on the total amount.

**Q: How do I record a donation for a charity?**
Use the `track_donations` tool and set the `isCharityDonation` flag to true to ensure funds are tracked separately from event costs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/memorial-event-planner](https://vinkius.com/en/ai-agent-connect/memorial-event-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Memorial Event Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `memorial-event-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Memorial Event Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "memorial-event-planner": {
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
