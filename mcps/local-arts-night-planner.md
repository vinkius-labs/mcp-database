# Local Arts Night Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-arts-night-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Orchestrates optimal itineraries for arts events based on time, venue, and accessibility constraints.

## Description
This MCP server acts as an intelligent scheduler for evening arts outings. It uses `plan_arts_sequence` to generate chronological itineraries that respect travel times, user pace, and accessibility needs. It also provides `validate_travel_feasibility` to check movement between venues, `check_ticket_availability` to manage reservations, and `get_fallback_option` to suggest alternatives if a full plan is not possible.


## Available Tools (4)
- **plan_arts_sequence**: Generates the optimal itinerary and necessary logistical messages based on user constraints
- **validate_travel_feasibility**: Checks if the user can move between two specific venues using their available transport within a given time window
- **check_ticket_availability**: Determines if an event requires immediate reservation or can be attended via walk-in
- **get_fallback_option**: Identifies the best single alternative when a full sequence cannot be constructed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Arts Night Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan an arts night starting at 18:00 with a relaxed pace, including wheelchair access."

**🤖 AI Agent:**
> Your itinerary: 18:00 Modern Gallery (Wheelchair accessible), followed by 20:30 Jazz Lounge. Please reserve tickets for the Modern Gallery now.

---

**👤 You:**
> "Can I get from the Museum to the Theater by subway in 20 minutes?"

**🤖 AI Agent:**
> Yes, traveling by subway between the Museum and the Theater is feasible within your 20-minute window.

---

**👤 You:**
> "Do I need to book tickets for the street art walk?"

**🤖 AI Agent:**
> No, the street art walk is open entry, so you can walk in whenever you arrive.


## ❓ FAQ

**Q: How does the planner handle travel time?**
The system uses `validate_travel_feasibility` to ensure you can move between venues. It adjusts travel time based on your `desiredPace`, such as allowing more buffer for a 'relaxed' pace.

**Q: Can I plan for specific accessibility needs?**
Yes. The `plan_arts_sequence` tool filters all options to ensure every event in your sequence meets your specified `accessibilityRequirements`.

**Q: What happens if my preferred sequence isn't possible?**
If constraints like time or transport prevent a full sequence, the tool `get_fallback_option` identifies the best single alternative that still meets your requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-arts-night-planner](https://vinkius.com/en/ai-agent-connect/local-arts-night-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Arts Night Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-arts-night-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Arts Night Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-arts-night-planner": {
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
