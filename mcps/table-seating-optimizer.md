# Table Seating Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/table-seating-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Calculate venue capacity, table layouts, and space requirements for events.

## Description
The Table Seating Optimizer is an advanced engine designed to help event planners maximize venue utility. By using tools like `calculate_max_capacity`, you can determine the highest guest count possible for any room dimension. The `generate_layout_grid` tool provides precise rows and columns for table placement, while `estimate_required_space` helps you plan the minimum square footage needed for your target guest list. All calculations adhere to industry standards, including a 42-inch clearance between tables and dedicated dance floor allocations.


## Available Tools (3)
- **estimate_required_space**: Estimate the minimum venue size required
- **generate_layout_grid**: Generate the table arrangement grid
- **calculate_max_capacity**: Calculate the maximum number of guests that can be accommodated in a room


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Table Seating Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the maximum capacity for a 50x100 ft room with 60-inch rounds and a 500 sq ft dance floor?"

**🤖 AI Agent:**
> The maximum capacity is 420 guests, utilizing 18 tables in the layout.

---

**👤 You:**
> "How much space do I need for 200 guests using rectangular tables and a 10 sq ft per person dance floor requirement?"

**🤖 AI Agent:**
> You will need a minimum of 4,500 square feet to accommodate the seating and the required 2,000 sq ft dance floor.

---

**👤 You:**
> "Generate a layout grid for a 40x60 room with 8-person rounds and a 200 sq ft dance floor."

**🤖 AI Agent:**
> The layout will consist of 3 rows and 4 columns of tables.


## ❓ FAQ

**Q: How does the clearance rule work?**
The engine enforces a standard 42-inch separation between the edges of adjacent tables to ensure proper chair clearance and movement.

**Q: Can I plan for a dance floor?**
Yes, you can specify the required square footage for a dance floor, and the tools will automatically subtract this area from the usable room space.

**Q: What table types are supported?**
The system supports various configurations, including round and rectangular tables, defined by their physical dimensions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/table-seating-optimizer](https://vinkius.com/mcp/table-seating-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Table Seating Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `table-seating-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Table Seating Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "table-seating-optimizer": {
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
