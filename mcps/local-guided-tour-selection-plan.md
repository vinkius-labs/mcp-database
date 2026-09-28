# Local Guided Tour Selection Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-guided-tour-selection-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

An intelligent decision engine that filters and ranks local guided tours based on strict logistical constraints and personal preferences.

## Description
This MCP server acts as a specialized decision engine for travelers. It uses `filter_available_tours` to eliminate options that fail mandatory constraints like accessibility, scheduling, and group size. Once valid options are identified, `rank_preferred_tours` orders them by interest alignment. Finally, `generate_tour_itinerary_summary` provides a complete package including booking steps and meeting instructions, while `validate_meeting_logistics` ensures the meeting point is practical for your group.


## Available Tools (4)
- **generate_tour_itinerary_summary**: Generates a final itinerary summary, booking steps, and meeting instructions
- **rank_preferred_tours**: Ranks valid tours based on how well they match user interests
- **validate_meeting_logistics**: Validates if the meeting point and time are practical for the group
- **filter_available_tours**: Filters tours based on mandatory accessibility, schedule, language, and group size constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Guided Tour Selection Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need a wheelchair accessible tour in English for 4 people tomorrow morning."

**🤖 AI Agent:**
> I have found a suitable wheelchair accessible city tour starting at 10:00 AM tomorrow. It is available in English and accommodates up to 6 people.

---

**👤 You:**
> "Find me a tour focused on history for a group of 2."

**🤖 AI Agent:**
> The best match is the 'Ancient Ruins Walking Tour', which focuses heavily on historical landmarks.

---

**👤 You:**
> "Where should we meet for the mountain hike?"

**🤖 AI Agent:**
> You should meet at the North Trailhead entrance at 8:00 AM. Please arrive 15 minutes early to check in with the guide.


## ❓ FAQ

**Q: How does the engine handle accessibility requirements?**
The `filter_available_tours` tool checks every tour against your specific accessibility needs to ensure only suitable options are presented.

**Q: Can I get specific meeting instructions for my tour?**
Yes, the `generate_tour_itinerary_summary` tool provides clear meeting instructions, and `validate_meeting_logistics` checks if the location is practical for your group size.

**Q: What happens if no tours match my exact interests?**
The engine will still return valid tours that meet your hard constraints, such as language and accessibility, even if the interest score is low.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-guided-tour-selection-plan](https://vinkius.com/en/ai-agent-connect/local-guided-tour-selection-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Guided Tour Selection Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-guided-tour-selection-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Guided Tour Selection Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-guided-tour-selection-plan": {
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
