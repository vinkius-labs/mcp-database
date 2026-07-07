# Driving Shift Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/driving-shift-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [transportation](../categories/transportation.md)

Plan long-distance drives with mandatory rest periods.

## Description
The Driving Shift Planner MCP server helps drivers manage long journeys by splitting them into segments. Use tools like `get_driving_itinerary` to see a full schedule of driving and rest periods, or `verify_drive_compliance` to ensure your planned segment stays within legal limits.


## Available Tools (3)
- **verify_drive_compliance**: Verify if a planned drive time is compliant
- **calculate_total_duration**: Calculate the total time for a journey
- **get_driving_itinerary**: Calculate a driving itinerary with rest periods


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Driving Shift Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my schedule for a 500km trip at 100km/h with a 3-hour max drive time and 30-minute rests?"

**🤖 AI Agent:**
> Driver 1: 0h to 3h. Rest: 3h to 3:30h. Driver 2: 3:30h to 5:30h.

---

**👤 You:**
> "Is a 4-hour drive segment legal if my limit is 3 hours?"

**🤖 AI Agent:**
> No, that segment exceeds the maximum allowed driving duration.

---

**👤 You:**
> "What is the total time for a 1000km trip at 100km/h with 2-hour max drives and 45-minute rests?"

**🤖 AI Agent:**
> The total elapsed time including all mandatory rest periods is 13 hours.


## ❓ FAQ

**Q: How can I see my full trip schedule?**
Use the `get_driving_itinerary` tool with your total distance and speed.

**Q: Can it check if a specific drive time is legal?**
Yes, use `verify_drive_compliance` to check against maximum allowed hours.

**Q: Does it include rest breaks?**
Yes, the itinerary includes all mandatory rest periods required by your settings.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/driving-shift-planner](https://vinkius.com/mcp/driving-shift-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Driving Shift Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `driving-shift-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Driving Shift Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "driving-shift-planner": {
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
