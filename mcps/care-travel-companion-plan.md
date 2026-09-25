# Care Travel Companion Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-travel-companion-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Coordinates care-specific travel timelines, packing responsibilities, and emergency fallback plans.

## Description
This MCP server transforms travel itineraries and care requirements into actionable support structures. It manages connection buffers for mobility needs, ensures document custody through responsibility mapping, and generates contingency plans for disruptions. Use `get_support_timeline` to schedule transitions, `get_packing_responsibilities` to assign items to travelers or companions, `get_contact_card` for emergency summaries, and `get_disruption_plan` to prepare for travel interruptions.


## Available Tools (4)
- **get_disruption_plan**: Formulates a contingency strategy based on the traveler's needs and current bookings
- **get_contact_card**: Produces a consolidated information sheet for the approved companion and emergency contacts
- **get_packing_responsibilities**: Creates a split list of items that must be packed by the traveler versus the companion
- **get_support_timeline**: Generates a chronological schedule of care-specific milestones and transition windows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Travel Companion Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a support timeline for a traveler with a 30-minute mobility buffer between airport arrival and hotel check-in."

**🤖 AI Agent:**
> The adjusted schedule includes a 30-minute buffer after arrival, setting the hotel check-in window to start at 14:30.

---

**👤 You:**
> "Who needs to pack the wheelchair and the medical insurance papers?"

**🤖 AI Agent:**
> The wheelchair and medical insurance papers are assigned to the Companion-Managed responsibility tier.

---

**👤 You:**
> "Create an emergency contact card for the companion and transport providers."

**🤖 AI Agent:**
> The contact card has been generated, including the companion's identity, traveler medical alerts, and direct contact info for all transport providers.


## ❓ FAQ

**Q: How does this tool handle mobility constraints?**
The `get_support_timeline` tool applies connection buffers to transitions, ensuring travelers with mobility needs have sufficient time between activities.

**Q: Who is responsible for medical documents?**
Using `get_packing_responsibilities`, all documents and accessibility requests are automatically assigned to the 'Companion-Managed' tier to ensure proper document custody.

**Q: Can I prepare for flight delays?**
Yes, `get_disruption_plan` generates contingency strategies that respect specific accessibility requests during transport failures or medical delays.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-travel-companion-plan](https://vinkius.com/en/ai-agent-connect/care-travel-companion-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Travel Companion Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-travel-companion-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Travel Companion Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-travel-companion-plan": {
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
