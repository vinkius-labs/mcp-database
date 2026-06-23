# SolarAnywhere API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/solaranywhere-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Monitor solar data — audit irradiance and sites via AI.

## Description
Empower your AI agent to orchestrate your entire solar energy research and site auditing workflow with **SolarAnywhere**, the authoritative source for high-resolution solar irradiance data. By connecting the SolarAnywhere API to your agent, you transform complex meteorological searches into a natural conversation. Your agent can instantly retrieve real-time irradiance levels, audit typical meteorological year (TMY) data, and query specific site metadata without you ever touching a technical portal. Whether you are conducting renewable energy research or managing regional solar fleet constraints, your agent acts as a real-time solar consultant, ensuring your data is always verified and precise.

### What you can do

- **Irradiance Auditing** — Retrieve real-time Global Horizontal Irradiance (GHI) and Direct Normal Irradiance (DNI) data for any coordinate pair instantly.
- **Site Oversight** — Audit all registered solar sites in your catalog to maintain a clear view of regional distribution and scale.
- **Weather Discovery** — Query Typical Meteorological Year (TMY) data to understand long-term solar potential for your energy projects.
- **Atmospheric Intelligence** — Retrieve temperature and irradiance metadata to assist in deep-dive solar performance classification.
- **Operational Monitoring** — Check API status to ensure your solar research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your SolarAnywhere API Key
3. Start managing your solar intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Solar Engineers & Analysts** — monitor site performance and retrieve official irradiance metadata straight from your workflow.
- **Renewable Energy Developers** — verify solar potential and audit TMY patterns without manual searching.
- **Sustainability Leads** — perform rapid audits of solar assets and identify relevant environmental markers through natural language.
- **Operations Leads** — automate solar data querying to orchestrate cross-functional energy teams smoothly.


## Available Tools (4)
- **check_api_status**: Check if the SolarAnywhere service is operational
- **get_solar_irradiance**: Get real-time solar irradiance data for a specific location
- **get_typical_solar_year**: Get Typical Meteorological Year (TMY) solar data for a location
- **list_solar_sites**: List all solar sites registered in your SolarAnywhere account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SolarAnywhere API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get solar irradiance for latitude 34.0522 and longitude -118.2437 using SolarAnywhere."

**🤖 AI Agent:**
> I've retrieved the real-time solar data! The Global Horizontal Irradiance (GHI) is currently 850 W/m² and the temperature is 25°C. Would you like the full DNI and DHI metadata for these coordinates?

---

**👤 You:**
> "Show Typical Meteorological Year data for 'Napa Valley'."

**🤖 AI Agent:**
> I've identified the coordinates for Napa Valley and retrieved the TMY data. The long-term solar potential is identified as having a high consistency for energy production. I can provide the monthly average irradiance metadata if you'd like.

---

**👤 You:**
> "List all registered solar sites in my account."

**🤖 AI Agent:**
> I've retrieved the site catalog from SolarAnywhere! You have 5 registered sites, including 'Solar-West-Alpha' and 'Utility-One'. I can provide the exact coordinate metadata and GHI data for any of these sites.


## ❓ FAQ

**Q: How do I find my SolarAnywhere API Key?**
Log in to your [**SolarAnywhere account**](https://api.solaranywhere.com/account), and you will find your API Key in your dashboard or profile settings. Copy and paste it below.

**Q: What irradiance parameters are provided?**
The API provides Global Horizontal Irradiance (GHI), Direct Normal Irradiance (DNI), and Diffuse Horizontal Irradiance (DHI) metadata.

**Q: Can the agent show historical typical year data?**
Yes. The `get_typical_solar_year` tool retrieves TMY data for any coordinate pair to assist in long-term performance auditing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/solaranywhere-api](https://vinkius.com/mcp/solaranywhere-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SolarAnywhere API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `solaranywhere-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SolarAnywhere API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "solaranywhere-api": {
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
