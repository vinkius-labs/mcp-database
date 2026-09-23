# Outdoor Chair Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/outdoor-chair-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Calculate precise chair and table requirements for outdoor events.

## Description
This MCP server provides event planners with essential tools to manage seating logistics. Use `get_required_chair_count` to determine total seating needs, `get_table_configuration` to plan table layouts, and `validate_event_capacity` to check if current inventory meets guest requirements. It also provides a `get_chair_distribution_summary` to understand how guests will be spread across tables.


## Available Tools (4)
- **get_chair_distribution_summary**: Provides a breakdown of how chairs will be distributed across the table layout
- **get_required_chair_count**: Calculates the total number of chairs needed for an event
- **get_table_configuration**: Determines how many tables of a specific type are needed for a given guest count
- **validate_event_capacity**: Checks if a specific set of existing furniture can accommodate a planned guest count


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Outdoor Chair Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many chairs do I need for 100 guests if each table holds 8 people? Include a buffer of 5 chairs."

**🤖 AI Agent:**
> You will need 109 chairs in total (13 tables of 8, plus a 5 chair buffer).

---

**👤 You:**
> "I have 40 chairs and 8 tables that seat 4 people each. Can I host 40 guests?"

**🤖 AI Agent:**
> Yes, your current inventory is sufficient to accommodate 40 guests.

---

**👤 You:**
> "Show me the table distribution for 25 guests with 6 chairs per table."

**🤖 AI Agent:**
> There will be 4 full tables and 1 partially filled table with 1 guest.


## ❓ FAQ

**Q: How do I calculate the total number of chairs needed?**
You can use the `get_required_chair_count` tool by providing the guest count, the capacity of each table, and an optional buffer margin.

**Q: Can I check if my current inventory is sufficient?**
Yes, the `validate_event_capacity` tool allows you to compare your guest count against your available chairs and tables to identify any shortages.

**Q: How many tables will I need for 50 guests with 4-person tables?**
Using `get_table_configuration` with 50 guests and 4 chairs per table, you will need 13 tables.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/outdoor-chair-counter](https://vinkius.com/en/ai-agent-connect/outdoor-chair-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Outdoor Chair Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `outdoor-chair-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Outdoor Chair Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "outdoor-chair-counter": {
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
