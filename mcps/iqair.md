# IQAir MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/iqair)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Monitor air quality and weather — audit pollution data and cities via AI.

## Description
Empower your AI agent to orchestrate your entire environmental research and air quality auditing workflow with **IQAir**, the world's most popular platform for air quality data. By connecting the AirVisual API to your agent, you transform complex pollution searches into a natural conversation. Your agent can instantly retrieve real-time air quality indices (AQI), audit weather conditions, and identify the most polluted areas without you ever touching a technical portal. Whether you are conducting climate research or monitoring local health constraints, your agent acts as a real-time environmental assistant, ensuring your data is always precise and localized.

### What you can do

- **Pollution Auditing** — Retrieve real-time Air Quality Index (AQI) data for the nearest city or specific global locations instantly.
- **Weather Oversight** — Audit current weather conditions, including temperature, humidity, and atmospheric pressure, to maintain a clear view of environmental scale.
- **Geographic Discovery** — List all supported countries, states, and cities in the IQAir catalog to understand the geographic reach of air quality monitoring.
- **Local Intelligence** — Query specific city data to understand local pollution markers and main pollutants (e.g., p2, p1).
- **Operational Monitoring** — Check API status to ensure your environmental research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your IQAir API Key
3. Start managing your environmental intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Environmental Researchers** — monitor pollution patterns and retrieve official metadata straight from your workflow.
- **Health Professionals** — verify local air quality and audit pollution trends for respiratory health assessments.
- **Sustainability Leads** — perform rapid audits of corporate locations and identify environmental hotspots through natural language.
- **Operations Leads** — automate atmospheric data querying to orchestrate cross-functional climate teams smoothly.


## Available Tools (6)
- **list_supported_cities**: List all cities supported for a specific state and country
- **list_supported_countries**: List all countries supported by IQAir
- **list_supported_states**: List all states supported for a specific country
- **check_api_status**: Check if the IQAir API is operational
- **get_city_air_quality**: Get real-time air quality and weather for a specific city
- **get_nearest_city_air_quality**: Get real-time air quality and weather for the city nearest to the requester IP


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IQAir** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the air quality in 'Los Angeles, California, USA' using IQAir?"

**🤖 AI Agent:**
> I've retrieved the real-time data for Los Angeles. The Air Quality Index (AQI) is currently 45, which is identified as 'Good'. The weather is 22°C with 60% humidity. Would you like the data for other cities in California?

---

**👤 You:**
> "Check air quality for my nearest city."

**🤖 AI Agent:**
> I've identified the nearest monitored city via your IP! The air quality is currently 'Moderate' with an AQI of 65. The main pollutant is identified as PM2.5. I can provide the full weather breakdown if you'd like.

---

**👤 You:**
> "List all cities supported in the state of 'Sao Paulo', Brazil."

**🤖 AI Agent:**
> I've scanned the catalog for Sao Paulo. It includes over 20 monitored cities, such as Sao Paulo city, Campinas, and Santos. I can retrieve the real-time AQI for any of these locations.


## ❓ FAQ

**Q: How do I find my IQAir API Key?**
Log in to your [**IQAir dashboard**](https://www.iqair.com/dashboard/api), create a new key in the API section, and copy it. Copy and paste it below.

**Q: Does the agent use the server's IP for nearest city?**
Yes. The `get_nearest_city_air_quality` tool automatically uses the requester's IP address to identify and audit the nearest monitored location.

**Q: Are weather details included with air quality?**
Yes. Every city data retrieval includes current weather metadata such as temperature, humidity, and atmospheric pressure alongside the AQI.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/iqair](https://vinkius.com/mcp/iqair)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IQAir** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `iqair` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IQAir** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "iqair": {
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
