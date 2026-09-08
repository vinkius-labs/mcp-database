# Haul Road Design Engineer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/haul-road-design-engineer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Design safe and efficient haul roads for open-pit mining operations.

## Description
This MCP server provides specialized engineering tools for designing haul roads in open-pit mines. It calculates critical dimensions such as road width and curve radius, ensures safety through sight distance analysis, and defines structural requirements for surfacing and drainage. Use `calculate_road_geometry` to determine physical dimensions, `calculate_curve_and_sight` for safety parameters, `design_surface_and_drainage` for structural needs, and `estimate_maintenance_schedule` to predict upkeep requirements.


## Available Tools (4)
- **calculate_curve_and_sight**: Ensures turns are safe for the vehicle speed and that drivers can see far enough ahead to stop
- **calculate_road_geometry**: Determines the physical dimensions required for a specific vehicle and traffic profile
- **design_surface_and_drainage**: Defines the structural and water-management needs of the road
- **estimate_maintenance_schedule**: Predicts the frequency of required road upkeep


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Haul Road Design Engineer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the road geometry for a 7-meter wide truck with 50 vehicles per hour on a two-way road with a 5% gradient."

**🤖 AI Agent:**
> The total road width required is 18.5 meters, including a safety berm width of 3.5 meters and a running surface width of 15.0 meters.

---

**👤 You:**
> "What is the required sight distance for a truck with a width of 6 meters traveling at 40 km/h on a 3% gradient?"

**🤖 AI Agent:**
> The required sight distance is 85 meters, with a minimum curve radius of 55 meters.

---

**👤 You:**
> "Design the surface for a road with 100 vehicles per hour, 250 tonne trucks, and 1200mm annual rainfall."

**🤖 AI Agent:**
> The recommended surface material is Tier 1 (High Performance) with a cross-fall degree of 2.5% and a standard ditch requirement.


## ❓ FAQ

**Q: What parameters are needed for road geometry?**
You need to provide the truck width, traffic volume, whether it is a two-way road, and the gradient.

**Q: How does the tool handle safety requirements?**
The `calculate_curve_and_sight` tool calculates the minimum curve radius and required sight distance based on vehicle width, design speed, and gradient.

**Q: Can I estimate maintenance costs?**
Yes, using `estimate_maintenance_schedule`, you can predict the maintenance interval and estimated annual cost based on traffic and truck weight.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/haul-road-design-engineer](https://vinkius.com/ai-agent-connect/haul-road-design-engineer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Haul Road Design Engineer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `haul-road-design-engineer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Haul Road Design Engineer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "haul-road-design-engineer": {
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
