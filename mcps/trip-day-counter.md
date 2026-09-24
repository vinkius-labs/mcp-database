# Trip Day Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/trip-day-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculates exact travel durations between departure and return dates.

## Description
This MCP server provides precise tools for travel itinerary management. Use `get_trip_duration` to find the total days in a trip, `validate_itinerary_dates` to ensure your travel dates are chronological, `get_trip_summary` for a high-level overview, or `find_longest_trip` to identify the longest segment in a collection of trips.


## Available Tools (4)
- **find_longest_trip**: Identifies the longest trip from a provided collection of trip segments
- **get_trip_duration**: Calculates the total number of days for a single trip
- **validate_itinerary_dates**: Checks if a set of dates is logically sound for travel
- **get_trip_summary**: Provides a high-level overview of a trip's span


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Trip Day Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many days is my trip from 2024-06-01 to 2024-06-05?"

**🤖 AI Agent:**
> Your trip lasts 5 days.

---

**👤 You:**
> "Give me a summary for a trip from 2024-12-20 to 2025-01-05."

**🤖 AI Agent:**
> Departure: 2024-12-20, Return: 2025-01-05, Total Days: 17.

---

**👤 You:**
> "Which is the longest trip: [{'departureDate': '2024-01-01', 'returnDate': '2024-01-05'}, {'departureDate': '2024-02-01', 'returnDate': '2024-02-10'}]?"

**🤖 AI Agent:**
> The longest trip is from 2024-02-01 to 2024-02-10, lasting 10 days.


## ❓ FAQ

**Q: How is the trip duration calculated?**
The duration is calculated by finding the difference between the departure and return dates and including both days in the count.

**Q: What date format should I use?**
All dates must be provided in the YYYY-MM-DD format.

**Q: Can I validate multiple dates at once?**
Yes, you can use `validate_itinerary_dates` to check if a list of dates follows a logical chronological sequence.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/trip-day-counter](https://vinkius.com/en/ai-agent-connect/trip-day-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Trip Day Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `trip-day-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Trip Day Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "trip-day-counter": {
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
