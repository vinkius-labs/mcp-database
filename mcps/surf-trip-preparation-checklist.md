# Surf Trip Preparation Checklist MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surf-trip-preparation-checklist)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate comprehensive surf trip checklists including gear, documents, and schedules.

## Description
This MCP server provides a complete planning engine for surfing expeditions. It uses specialized tools like `get_equipment_checklist` to determine gear based on wave conditions and board count, `get_travel_documents` to identify legal requirements, and `get_timing_schedule` to organize trip milestones. It ensures surfers are prepared for any environment, from mellow beach breaks to heavy reef swells.


## Available Tools (4)
- **get_equipment_checklist**: Determines exactly what gear a surfer needs to pack based on the environment and their board count
- **get_travel_documents**: Identifies the necessary legal and identification requirements for the trip
- **get_timing_schedule**: Generates a chronological timeline of activities leading up to and during the trip
- **get_trip_summary**: Provides a high-level overview of the entire plan in one view


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surf Trip Preparation Checklist** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I'm going to Bali for 10 days with 2 boards. The waves will be heavy reef swells. What should I pack?"

**🤖 AI Agent:**
> For your 10-day trip to Bali with heavy reef swells, you will need: Essential: 2 surfboards, impact vest, and a thick wetsuit. Secondary: Wax, leashes, and fins. Backup: Spare fins and a repair kit.

---

**👤 You:**
> "What documents do I need for a trip to Portugal?"

**🤖 AI Agent:**
> For Portugal, you will need your Passport as a mandatory document. It is also recommended to carry Travel Insurance and your Vaccination records.

---

**👤 You:**
> "Give me a summary for a 7-day trip to Costa Rica with mellow beach breaks and 1 board."

**🤖 AI Agent:**
> Your trip to Costa Rica summary: Destination: Costa Rica, Duration: 7 days, Gear Count: 8 items, Document Count: 2 items, Schedule Complexity: Moderate.


## ❓ FAQ

**Q: How does the gear checklist work?**
The `get_equipment_checklist` tool analyzes your destination, the expected wave conditions, and how many boards you are bringing to provide a tailored list of essential, secondary, and backup gear.

**Q: Can I plan my trip timeline?**
Yes, you can use `get_timing_schedule` to generate a chronological timeline of preparation milestones and a daily routine for the duration of your trip.

**Q: Does it cover travel documents?**
Yes, the `get_travel_documents` tool identifies mandatory and recommended documentation required for your specific destination.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surf-trip-preparation-checklist](https://vinkius.com/en/ai-agent-connect/surf-trip-preparation-checklist)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surf Trip Preparation Checklist** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surf-trip-preparation-checklist` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surf Trip Preparation Checklist** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surf-trip-preparation-checklist": {
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
