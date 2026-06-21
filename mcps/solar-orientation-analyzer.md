# Solar Orientation Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/solar-orientation-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [architecture](../categories/architecture.md)

Calculate solar incidence angles, sunlight duration, and architectural protection strategies based on building orientation and latitude.

## Description
The Solar Orientation Analyzer provides specialized tools for architects and engineers to assess solar exposure. Use `calculate_solar_incidence` to determine the sun's angle relative to a facade during summer, winter, and equinox periods. Use `estimate_sunlight_duration` to calculate how many hours of direct sunlight each face receives throughout the year. Finally, use `generate_protection_srategy` to receive architectural recommendations like brise-soleil or reflective glazing based on calculated heat gain risks.


## Available Tools
- **generate_protection_strategy**: Returns recommendation and impact level.

Provides architectural recommendations for solar shading or heat mitigation based on calculated exposure
- **calculate_solar_incidence**: Returns angles for summer, winter, and equinox.

Determines the estimated angle of the sun relative to a specified building facade during different seasonal periods
- **estimate_sunlight_duration**: Returns duration in hours for summer, winter, and equinox.

Estimates how many hours of direct, unshaded sunlight a specific facade receives during different seasons


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Solar Orientation Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the solar incidence for a North facing facade in Brasilia?"

**🤖 AI Agent:**
> The `calculate_solar_incidence` tool would provide the specific angles for summer, winter, and equinox based on Brasilia's latitude.

---

**👤 You:**
> "How many hours of sun does an East facing facade get in Sao Paulo?"

**🤖 AI Agent:**
> Using `estimate_sunlight_duration`, you can find the estimated hours of direct sunlight for that orientation during different seasons.

---

**👤 You:**
> "Suggest a protection strategy for a West facing facade in Fortaleza."

**🤖 AI Agent:**
> The `generate_protection_strategy` tool will evaluate the high solar exposure and recommend appropriate architectural interventions.


## ❓ FAQ

**Q: What inputs are required for the tools?**
You need to provide the facade orientation (in degrees or cardinal points like 'North') and a Brazilian capital city name to retrieve the necessary latitude.

**Q: How does it calculate solar incidence?**
The `calculate_solar_incidence` tool uses the latitude of the provided city to estimate the sun's angle relative to your facade during summer, winter, and equinox seasons.

**Q: Can I get architectural recommendations?**
Yes, the `generate_protection_strategy` tool analyzes exposure levels to suggest mitigation techniques like louvers or shading devices.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/solar-orientation-analyzer](https://vinkius.com/mcp/solar-orientation-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Solar Orientation Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `solar-orientation-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Solar Orientation Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "solar-orientation-analyzer": {
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
