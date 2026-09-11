# Air Quality Dispersion Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/air-quality-dispersion-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industrial](../categories/industrial.md)

Predict pollutant dispersion and ground-level concentrations from industrial sources.

## Description
This MCP server provides specialized modeling tools for predicting how air pollutants disperse from oil and gas facilities. It uses Gaussian plume logic to calculate ground-level concentrations, identify the point of maximum impact, and assess risks like building downwash. Users can also adjust predictions for complex terrain to ensure compliance with ambient air quality standards.


## Available Tools (4)
- **analyze_terrain_effects**: Adjusts dispersion predictions based on the presence of hills or valleys
- **calculate_ground_concentration**: Determines the concentration of a pollutant at a specific geographic coordinate
- **estimate_maximum_impact**: Identifies the point of highest pollutant concentration and its distance from the source
- **evaluate_downwash_risk**: Assesses how much a nearby structure will disrupt the plume and increase ground-level concentrations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Air Quality Dispersion Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the pollutant concentration at latitude 34.05 and longitude -118.24 if the emission rate is 50 g/s, stack height is 50m, wind speed is 3 m/s, and stability class is D?"

**🤖 AI Agent:**
> The predicted ground-level concentration at the specified coordinates is 12.5 µg/m³.

---

**👤 You:**
> "Where will the maximum pollutant impact occur for an emission rate of 100 g/s, 60m stack, 5 m/s wind, and 400K stack temperature?"

**🤖 AI Agent:**
> The maximum concentration will occur at a distance of 1,250 meters from the source in a direction of 180 degrees.

---

**👤 You:**
> "Is there a downwash risk if a 50m stack is near a 40m wide building with a height of 30m and wind speed of 4 m/s?"

**🤖 AI Agent:**
> The risk level is moderate, with an expected concentration multiplier of 1.4 due to building downwash.


## ❓ FAQ

**Q: How do I calculate the concentration at a specific location?**
You can use the `calculate_ground_concentration` tool by providing the emission rate, stack height, wind speed, target coordinates, and atmospheric stability class.

**Q: Can this model account for nearby buildings?**
Yes, the `evaluate_downwash_risk` tool assesses how nearby structures disrupt the plume and increase ground-level concentrations.

**Q: Does it work for hilly or mountainous areas?**
Yes, you can use `analyze_terrain_effects` to adjust your dispersion predictions based on elevation changes and complex terrain.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/air-quality-dispersion-model](https://vinkius.com/en/ai-agent-connect/air-quality-dispersion-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Air Quality Dispersion Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `air-quality-dispersion-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Air Quality Dispersion Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "air-quality-dispersion-model": {
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
