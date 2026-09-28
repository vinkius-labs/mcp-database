# Heritage Rail Experience Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/heritage-rail-experience-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Coordinate heritage rail journeys by synthesizing timetables, accessibility needs, and operator rules.

## Description
This MCP server acts as a coordination engine for heritage railway travel. It reconciles rigid operator rules with specific traveler requirements to produce cohesive journey plans. Use `plan_heritage_journey` to generate itineraries, `validate_boarding_strategy` to ensure station accessibility compliance, `calculate_ticket_and_companion_requirements` for booking logistics, and `generate_contingency_plan` to prepare for service disruptions.


## Available Tools (4)
- **generate_contingency_plan**: Provides a fallback option if the primary ride is unavailable or cancelled
- **plan_heritage_journey**: Generates the primary itinerary and logistical strategy for the trip
- **validate_boarding_strategy**: Ensures the proposed boarding actions are compliant with both station capabilities and accessibility needs
- **calculate_ticket_and_companion_requirements**: Determines the specific ticket types and companion needs to fulfill the booking


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Heritage Rail Experience Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a scenic heritage rail trip for a passenger with wheelchair access needs."

**🤖 AI Agent:**
> The selected ride is the Blue Valley Steam Express at 10:00 AM, which features level boarding for wheelchairs.

---

**👤 You:**
> "Check if the boarding strategy is viable for a station with steep stairs."

**🤖 AI Agent:**
> The boarding strategy is not viable because the station lacks step-free access required for the passenger's mobility profile.

---

**👤 You:**
> "Calculate the tickets needed for a passenger with a disability and a companion."

**🤖 AI Agent:**
> You will need one Adult Standard ticket and one Carer/Companion ticket.


## ❓ FAQ

**Q: How does the tool handle accessibility needs?**
The `validate_boarding_strategy` tool checks station infrastructure against specific mobility or sensory requirements to ensure the plan is viable.

**Q: Can I plan for companion discounts?**
Yes, `calculate_ticket_and_companion_requirements` identifies necessary companion ticket types based on passenger profiles and ticket terms.

**Q: What happens if my primary train is cancelled?**
You can use `generate_contingency_plan` to find an alternative ride that still respects your non-negotiable must-haves.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/heritage-rail-experience-planner](https://vinkius.com/en/ai-agent-connect/heritage-rail-experience-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Heritage Rail Experience Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `heritage-rail-experience-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Heritage Rail Experience Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "heritage-rail-experience-planner": {
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
