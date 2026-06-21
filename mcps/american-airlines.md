# American Airlines MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/american-airlines)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

AI flight tracking: check flight status, schedules, and airport info via agents.

## Description
### What you can do

Connect AI agents to the American Airlines API for real-time flight tracking and airport information:

- **Track Flight Status** in real-time (On Time, Delayed, Cancelled) for any AA flight
- **View Flight Schedules** between any two airports served by American Airlines
- **Get Airport Info** including terminal layouts and available services
- **Plan Travel** by comparing schedules and finding alternative flights

### How it works

1. **Get your API key** from the [American Airlines Developer Portal](https://developer.aa.com/)
2. **Ask your AI agent** to check flight status, view schedules, or get airport details
3. **Natural language commands** replace manual app navigation
4. **Real-time data** directly from AA's operational systems

### Who is this for?

Essential for **frequent travelers**, **travel agents**, **airport staff**, and **flight enthusiasts**. Let AI agents monitor flight delays, plan trips by comparing schedules, and provide terminal information. Perfect for anyone flying American Airlines who wants instant status updates and schedule visibility through natural language.


## Available Tools
- **get_airport_info**: Useful for checking terminal layouts or finding specific amenities at a hub airport.

Get information about an airport served by American Airlines
- **get_flight_schedule**: Returns flight numbers, departure/arrival times, aircraft types, and service classes. Use this to plan travel, find alternative flights if one is full, or compare schedule options.

Get flight schedule between two airports on a specific date
- **get_flight_status**: Use this to track your flight, check on a relative's arrival, or monitor delays. Requires flight number (e.g., 123 or AA123) and date (YYYY-MM-DD).

Get real-time status of a specific American Airlines flight


## 💬 Prompt Examples

Here are some examples of how you can interact with the **American Airlines** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the status of flight AA100 from JFK to LHR today"

**🤖 AI Agent:**
> I'll pull the real-time status and gate information for flight AA100.

---

**👤 You:**
> "Show me all flights from Miami to Dallas tomorrow morning"

**🤖 AI Agent:**
> I'll list the flight schedule for MIA to DFW for tomorrow.

---

**👤 You:**
> "What terminals are available at Chicago O'Hare (ORD)?"

**🤖 AI Agent:**
> I'll get the terminal information and services for ORD airport.


## ❓ FAQ

**Q: Can I book flights using this MCP server?**
No, this server is for informational and tracking purposes only. It provides flight status, schedules, and airport info. Booking requires a separate commercial integration or using the AA website/app directly.

**Q: Which flights are supported?**
This API supports American Airlines and American Eagle flights. It provides data for flights operated by AA, including code-share flights where AA is the marketing carrier.

**Q: How do I get an API key?**
You can register for a free API key at the [American Airlines Developer Portal](https://developer.aa.com/). Once registered, create a new application to generate your key for testing and development.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/american-airlines](https://vinkius.com/mcp/american-airlines)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **American Airlines** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `american-airlines` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **American Airlines** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "american-airlines": {
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
