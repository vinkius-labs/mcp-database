# Restaurant Table Capacity Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/restaurant-table-capacity-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Calculate seating capacity, occupancy rates, and seating distributions.

## Description
This MCP server provides essential tools for restaurant management to handle seating logistics. Use `get_total_capacity` to find the maximum number of guests that can be seated, `analyze_seating_distribution` to understand how seats are spread across different table sizes, and `calculate_occupancy_rate` to monitor how full the venue is. You can also use `validate_table_configuration` to ensure your setup meets specific event requirements.


## Available Tools (4)
- **analyze_seating_distribution**: Provides a breakdown of how seating is distributed across different table sizes
- **calculate_occupancy_rate**: Determines how full the restaurant is based on current guest count and table configuration
- **get_total_capacity**: Calculates the overall number of people that can be seated in the restaurant
- **validate_table_configuration**: Checks if a proposed table setup meets a minimum seating requirement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Restaurant Table Capacity Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total capacity for a restaurant with five 2-seater tables and three 4-seater tables?"

**🤖 AI Agent:**
> The total capacity is 22 seats.

---

**👤 You:**
> "If I have 22 total seats and 15 guests are currently seated, what is my occupancy rate?"

**🤖 AI Agent:**
> The occupancy rate is 68.18% with 7 seats remaining.

---

**👤 You:**
> "Does a setup of ten 2-seater tables meet a requirement of 25 seats?"

**🤖 AI Agent:**
> No, the configuration is invalid. There is a shortfall of 5 seats.


## ❓ FAQ

**Q: How do I calculate the total capacity?**
You can use the `get_total_capacity` tool by providing a JSON object where keys are the number of seats per table and values are the number of such tables.

**Q: Can I check if my restaurant is full?**
Yes, use the `calculate_occupancy_rate` tool with your current guest count and table configuration to see the occupancy percentage.

**Q: How can I verify if I have enough seats for an event?**
Use the `validate_table_configuration` tool to compare your current table setup against the minimum required seats for your event.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/restaurant-table-capacity-manager](https://vinkius.com/en/ai-agent-connect/restaurant-table-capacity-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Restaurant Table Capacity Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `restaurant-table-capacity-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Restaurant Table Capacity Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "restaurant-table-capacity-manager": {
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
