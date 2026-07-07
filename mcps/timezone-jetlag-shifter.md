# Timezone Jetlag Shifter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/timezone-jetlag-shifter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate a precise circadian adjustment schedule to mitigate jet lag before your international flight.

## Description
The Timezone Jetlag Shifter is a precision scheduling engine designed for travelers. It calculates a day-by-day itinerary of adjusted bedtimes and wake times leading up to your departure date. By using tools like `generate_shift_schedule`, you can plan your phase advance or phase delay based on your travel direction (east or west). The system also provides specific instructions via `identify_light_window` to optimize light exposure, helping your biological clock synchronize with your destination timezone efficiently.


## Available Tools (3)
- **generate_shift_schedule**: Generates a day-by-day circadian adjustment plan
- **calculate_timezone_difference**: Calculates the magnitude of time shift between two timezones
- **identify_light_window**: Provides light exposure instructions for a specific day


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Timezone Jetlag Shifter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am traveling from New York to London on June 15th. How should I adjust my sleep?"

**🤖 AI Agent:**
> Your adjustment schedule starts on June 12th. On June 12th, your bedtime will be 10:30 PM and wake time will be 6:30 AM.

---

**👤 You:**
> "What is the timezone difference between Tokyo and Los Angeles?"

**🤖 AI Agent:**
> The total time shift required is 17 hours.

---

**👤 You:**
> "When should I seek bright light for my trip to Paris?"

**🤖 AI Agent:**
> For your eastward travel, you should seek bright light in the morning hours on your target date.


## ❓ FAQ

**Q: How does the tool help with jet lag?**
It uses `generate_shift_schedule` to create a personalized sleep and light exposure plan for the days leading up to your trip.

**Q: Can I use it for westward travel?**
Yes, you can specify "west" as the direction to generate a phase delay schedule.

**Q: What information is needed?**
You need your departure date, home and destination timezones, and travel direction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/timezone-jetlag-shifter](https://vinkius.com/mcp/timezone-jetlag-shifter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Timezone Jetlag Shifter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `timezone-jetlag-shifter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Timezone Jetlag Shifter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "timezone-jetlag-shifter": {
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
