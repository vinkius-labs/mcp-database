# Photo Location Permission Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/photo-location-permission-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Generate production logistics, compliance checklists, and contact sheets for location shoots.

## Description
This MCP server provides production teams with essential tools to manage location logistics. Use `verify_location_readiness` to ensure equipment complies with property rules, `generate_permission_workflow` to plan owner communications, `map_production_logistics` to assign crew responsibilities and contingency plans, and `create_day_of_contact_sheet` to prepare for the shoot day.


## Available Tools (4)
- **create_day_of_contact_sheet**: Produces a concise reference document for the production day
- **generate_permission_workflow**: Creates the step-by-step communication plan needed to secure a location
- **map_production_logistics**: Defines who is responsible for what and what to do if things go wrong
- **verify_location_readiness**: Generates a checklist to ensure the location is fully prepared for the planned activity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Photo Location Permission Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if my camera gear and lighting kit are okay for the downtown studio given their no-tripod rule."

**🤖 AI Agent:**
> The downtown studio has a strict no-tripod rule. Your current equipment list includes a Manfrotto tripod, which violates the published restrictions. Please consider using a monopod or handheld stabilization instead.

---

**👤 You:**
> "Create a contact sheet for our shoot on October 12th at the Oak Park and Riverside Cafe."

**🤖 AI Agent:**
> Contact Sheet for October 12th:

Property Contacts:
- Oak Park: owner@oakpark.com
- Riverside Cafe: manager@riverside.com

Crew Contacts:
- Lead Producer: producer@production.com
- Camera Op: cam@production.com

Locations:
- Oak Park
- Riverside Cafe

---

**👤 You:**
> "What should we do if the weather ruins our shoot at the beach?"

**🤖 AI Agent:**
> In the event of weather-related site failure at the beach, you should immediately transition to the pre-approved alternate location: The Indoor Studio Loft.


## ❓ FAQ

**Q: How do I ensure my equipment is allowed at a location?**
You can use the `verify_location_readiness` tool. Provide the location name, planned activity, the property's published restrictions, and your equipment list to receive a compliance checklist.

**Q: Can I plan for backup locations if the primary site is unavailable?**
Yes. The `map_production_logistics` tool allows you to input alternate locations to generate specific contingency actions for your production.

**Q: How can I protect crew privacy when contacting property owners?**
Use the `generate_permission_workflow` tool and select a 'minimal' or 'standard' privacy level to redact sensitive crew details from initial outreach.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/photo-location-permission-planner](https://vinkius.com/en/ai-agent-connect/photo-location-permission-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Photo Location Permission Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `photo-location-permission-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Photo Location Permission Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "photo-location-permission-planner": {
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
