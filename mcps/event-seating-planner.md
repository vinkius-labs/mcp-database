# Event Seating Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/event-seating-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Deterministic venue capacity and seating layout calculator.

## Description
Plan your event with precision using the Event Seating Planner. This tool calculates maximum guest capacity based on fire code regulations and generates optimized seating arrangements. Use `calculate_capacity` to determine legal occupancy limits, `plan_seating_layout` to organize tables and dance floors, and `estimate_supplies` to get exact counts for linens and centerpieces.


## Available Tools (3)
- **calculate_capacity**: Determines the maximum legal and practical number of guests for a given venue and setup
- **estimate_supplies**: Provides the count of physical items needed to service the planned layout
- **plan_seating_layout**: Calculates the specific arrangement of tables, dance floor, and guest capacity based on furniture choices


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Event Seating Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the maximum capacity for a 50x100 foot venue with a 200 sq ft stage?"

**🤖 AI Agent:**
> The maximum capacity for a 50x100 foot venue with a 200 sq ft stage is 252 guests.

---

**👤 You:**
> "Plan a layout for a 40x60 foot room using 60 inch round tables and 8 guests per table."

**🤖 AI Agent:**
> The layout for a 40x60 foot room with 60 inch round tables accommodates 48 guests across 6 tables.

---

**👤 You:**
> "How many centerpieces do I need for 15 tables?"

**🤖 AI Agent:**
> You will need 15 centerpieces.


## ❓ FAQ

**Q: How does the tool calculate maximum capacity?**
The `calculate_capacity` tool evaluates both standing and seated occupancy limits based on the venue's usable area to ensure compliance with safety regulations.

**Q: Can I plan for different table types?**
Yes, `plan_seating_layout` supports round 60", round 72", rectangular 6ft, rectangular 8ft, and banquet table configurations.

**Q: How many linens do I need to order?**
You can use `estimate_supplies` to get the exact number of linens and centerpieces required based on your calculated table count.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/event-seating-planner](https://vinkius.com/ai-agent-connect/event-seating-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Event Seating Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `event-seating-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Event Seating Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "event-seating-planner": {
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
