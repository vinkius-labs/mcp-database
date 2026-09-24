# Itinerary Day Count MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/itinerary-day-count)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculates inclusive calendar days for travel itineraries.

## Description
This MCP server provides precise tools for managing travel timelines. Use `get_itinerary_duration` to find the total inclusive days of a trip, `validate_itinerary_range` to check if dates fall within specific seasonal bounds, `get_itinerary_summary` for a detailed temporal breakdown, or `compare_itineraries` to compare the lengths of two different trips.


## Available Tools (4)
- **compare_itineraries**: Compares the length of two different itineraries to determine which trip is longer
- **get_itinerary_duration**: Calculates the total number of inclusive calendar days for a single trip
- **get_itinerary_summary**: Provides a detailed breakdown of the itinerary's temporal footprint
- **validate_itinerary_range**: Checks if a given date range falls within a specific set of allowed travel constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Itinerary Day Count** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many days is my trip from 2024-07-01 to 2024-07-05?"

**🤖 AI Agent:**
> Your trip is 5 days long.

---

**👤 You:**
> "Is a trip from 2024-12-01 to 2024-12-01 valid?"

**🤖 AI Agent:**
> Yes, a trip where the start and end dates are the same is a valid 1-day itinerary.

---

**👤 You:**
> "Give me a summary for a trip from 2024-05-10 to 2024-05-15."

**🤖 AI Agent:**
> The trip lasts 6 days, it is not a single day trip, and there are 230 days remaining in the year after the trip ends.


## ❓ FAQ

**Q: How are the days counted?**
The count is inclusive of both the arrival day and the departure day. For example, arriving Monday and leaving Tuesday is a 2-day itinerary.

**Q: Can I compare two different trips?**
Yes, you can use `compare_itineraries` to determine which trip is longer and the exact difference in days.

**Q: What date format should I use?**
All dates must follow the standard ISO 8601 calendar format.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/itinerary-day-count](https://vinkius.com/en/ai-agent-connect/itinerary-day-count)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Itinerary Day Count** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `itinerary-day-count` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Itinerary Day Count** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "itinerary-day-count": {
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
