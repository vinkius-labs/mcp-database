# Accessible Station Navigation Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-station-navigation-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [accessibility](../categories/accessibility.md)

Generates step-by-step accessible transit itineraries and contingency plans.

## Description
This MCP server provides specialized tools for planning accessible transit journeys. It uses `get_station_navigation_plan` to create detailed arrival approaches and step-by-step directions based on specific station infrastructure and user needs. Users can also use `get_contingency_route` to find alternative paths if a primary entrance or elevator is unavailable, `validate_station_access` to verify station compatibility, and `calculate_buffer_impact` to determine necessary safety margins.


## Available Tools (4)
- **calculate_buffer_impact**: Calculates how much extra time the user needs to account for based on their specific equipment and the station's complexity
- **get_contingency_route**: Identifies a secondary accessible path if the primary entrance or elevator is unavailable
- **get_station_navigation_plan**: Generates a comprehensive transit plan including the approach, step-by-step directions, and assistance messaging
- **validate_station_access**: Verifies if a specific station configuration can support a user's specific equipment and needs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Station Navigation Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need a navigation plan for Central Station. I use a motorized wheelchair and need to arrive by 09:00. Please include a 10-minute safety margin."

**🤖 AI Agent:**
> Your arrival approach involves entering via the North Entrance. Step 1: Use the elevator at North Entrance. Step 2: Follow tactile paving to Platform 2. Your assistance request text: 'I am using a motorized wheelchair and require assistance at Platform 2 via the station radio channel.'

---

**👤 You:**
> "The main elevator at West Station is broken. Can you find me another way to the platform?"

**🤖 AI Agent:**
> The alternate entrance is the East Entrance. Follow the path through the South Concourse to reach the platform via the service elevator.

---

**👤 You:**
> "How much extra time should I add for a complex station with multiple transfers using a manual wheelchair?"

**🤖 AI Agent:**
> Based on a complexity score of 7 and ManualMobility equipment, a recommended buffer of 15 minutes is suggested.


## ❓ FAQ

**Q: How does the navigation plan account for my specific equipment?**
The `get_station_navigation_plan` tool uses your specific equipment details to ensure every step of the route, including elevator clearances and path widths, meets your requirements.

**Q: What happens if an elevator is out of service?**
You can use the `get_contingency_route` tool to identify the next most viable accessible entrance or elevator that bypasses the failed access point.

**Q: Can I check if a station is safe for my mobility aid before I travel?**
Yes, the `validate_station_access` tool verifies if a station configuration can support your specific equipment and assistance needs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-station-navigation-plan](https://vinkius.com/en/ai-agent-connect/accessible-station-navigation-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Station Navigation Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-station-navigation-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Station Navigation Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-station-navigation-plan": {
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
