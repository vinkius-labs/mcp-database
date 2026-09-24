# Hotel Room Night Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/hotel-room-night-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate total room nights based on occupancy and stay duration.

## Description
This MCP server provides tools to manage hotel inventory metrics. Use `calculate_stay_room_nights` to determine the total room nights for a single reservation, `compare_room_usage` to evaluate consumption between stays, `aggregate_group_room_nights` to sum totals for multiple bookings, and `validate_stay_bounds` to verify if dates fall within a specific period.


## Available Tools (4)
- **aggregate_group_room_nights**: 
- **calculate_stay_room_nights**: 
- **compare_room_usage**: 
- **validate_stay_bounds**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hotel Room Night Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the room nights for 3 rooms from 2024-05-01 to 2024-05-05."

**🤖 AI Agent:**
> The total room nights for this stay is 12.

---

**👤 You:**
> "Compare a stay with 10 room nights to a stay with 15 room nights."

**🤖 AI Agent:**
> The second stay is larger by 5 room nights.

---

**👤 You:**
> "Is a stay from 2024-06-01 to 2024-06-03 within the range 2024-05-01 to 2024-07-01?"

**🤖 AI Agent:**
> Yes, the stay is within the specified range.


## ❓ FAQ

**Q: How do I calculate room nights for a single guest?**
You can use the `calculate_stay_room_nights` tool by providing the number of rooms occupied and the check-in and check-out dates.

**Q: Can I sum up room nights for a whole group?**
Yes, the `aggregate_group_room_nights` tool allows you to sum the total room nights for a collection of different stays.

**Q: How can I check if a stay is within a specific date range?**
Use the `validate_stay_bounds` tool to verify if the arrival and departure dates fall within your specified range.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/hotel-room-night-calculator](https://vinkius.com/en/ai-agent-connect/hotel-room-night-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hotel Room Night Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hotel-room-night-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hotel Room Night Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hotel-room-night-calculator": {
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
