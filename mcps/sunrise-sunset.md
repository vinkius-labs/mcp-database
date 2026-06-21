# Sunrise-Sunset MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sunrise-sunset)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [scientific-research](../categories/scientific-research.md)

Get precise sunrise, sunset, and twilight times for any location on Earth using latitude and longitude coordinates.

## Description
Connect your AI agent to the **Sunrise-Sunset** API to retrieve accurate solar data for any location on Earth. Whether you are planning photography shoots, calculating energy potential, or managing outdoor events, this server provides the precise astronomical data you need.

### What you can do

- **Solar Events** — Get exact sunrise and sunset times for any latitude and longitude.
- **Twilight Phases** — Access civil, nautical, and astronomical twilight data for precise light level planning.
- **Day Length** — Retrieve the total duration of daylight for any given day.
- **Timezone Integration** — Get results in specific timezones using the `tzid` parameter.
- **Historical & Future Queries** — Look up solar data for any date, past or future.

### How it works

1. Subscribe to this server
2. Enter your API credentials
3. Start querying solar data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Photographers & Filmmakers** — plan the perfect 'golden hour' shots with exact twilight timings.
- **Energy Analysts** — calculate potential solar exposure based on day length and sun position.
- **Event Organizers** — ensure outdoor activities are scheduled with perfect lighting context.


## Available Tools
- **get_sunrise_sunset**: Get sunrise and sunset times for a location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sunrise-Sunset** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What time is the sunrise in London (51.5074, -0.1278) today?"

**🤖 AI Agent:**
> I've checked the solar data for London. Today, the sunrise is at 06:42 AM and the sunset will be at 05:58 PM. Would you like the twilight timings as well?

---

**👤 You:**
> "Get the sunset and civil twilight times for Paris on December 25th, 2025."

**🤖 AI Agent:**
> For Paris on Christmas Day 2025, the sunset is scheduled for 04:56 PM, with civil twilight ending at 05:34 PM. It will be a short day with a total length of 8 hours and 14 minutes.

---

**👤 You:**
> "Show me the day length for Los Angeles (34.0522, -118.2437) using the 'America/Los_Angeles' timezone."

**🤖 AI Agent:**
> In Los Angeles today, the total day length is 12 hours and 48 minutes. The sun rises at 06:12 AM and sets at 07:00 PM local time.


## ❓ FAQ

**Q: Can I get solar data for a specific date in the future?**
Yes! Use the `get_sunrise_sunset` tool and provide the `date` parameter in YYYY-MM-DD format (e.g., '2025-12-25').

**Q: Does the tool support local timezones?**
Yes. By providing a `tzid` (like 'Europe/London' or 'America/New_York'), the tool returns times adjusted for that specific region.

**Q: What is the difference between civil and astronomical twilight in the results?**
The `get_sunrise_sunset` tool returns all phases. Civil twilight is when there is still enough light for outdoor activities, while astronomical twilight marks when the sky is completely dark for astronomical observations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sunrise-sunset](https://vinkius.com/mcp/sunrise-sunset)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sunrise-Sunset** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sunrise-sunset` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sunrise-Sunset** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sunrise-sunset": {
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
