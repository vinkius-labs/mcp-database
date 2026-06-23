# Enverus Energy Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/enverus-energy-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Equip your AI agent to access global energy data, track drilling rigs, and monitor well production via the Enverus API.

## Description
Integrate **Enverus**, the leading energy SaaS company, directly into your AI workflow. Access real-time data on active drilling rigs and oil/gas wells, track new drilling permits and basin-specific activity, monitor M&A transactions in the energy sector, and oversee market intelligence using natural language.

### What you can do

- **Asset Oversight** — List and retrieve detailed information for active drilling rigs and oil/gas wells across various geological basins.
- **Production Intelligence** — Monitor well production telemetry, resolving daily BOE/d volumes and identifying gas-to-oil ratios.
- **Market Analysis** — Access high-level energy market summaries and recent M&A deal data to stay ahead of industry trends.
- **Energy Auditing** — Retrieve high-level summaries of rig counts, well activity, and organizational energy asset health instantly.

### How it works

1. Connect the Enverus integration to your AI assistant.
2. Authorize using your Enverus API Key (found in your account developer portal).
3. Orchestrate your energy research and market analysis through intuitive conversation.

### Who is this for?

- **Energy Analysts** — Quickly check rig locations and well production data on the go.
- **Investment Professionals** — Monitor sector-wide transactions and basin activity via chat.
- **Operations Teams** — Research drilling permits and organizational energy metadata instantly.


## Available Tools (10)
- **get_enverus_api_metadata**: Retrieve metadata and authorization status for your Enverus API connection
- **get_energy_market_intelligence_summary**: Retrieve a high-level summary of current energy market trends
- **quick_energy_asset_audit**: Retrieve a high-level summary of rig and well counts
- **get_rig_technical_details**: Get detailed settings and current activity for a specific rig
- **get_well_production_telemetry**: Get historical and current production data for a specific well
- **list_basin_specific_activity**: List rigs and wells active within a specific geological basin
- **list_drilling_permits**: List recently issued drilling permits
- **list_energy_m_and_a_deals**: List recent mergers, acquisitions, and asset transactions in the energy sector
- **list_active_drilling_rigs**: List all active drilling rigs currently tracked in the Enverus database
- **list_oil_and_gas_wells**: List oil and gas wells within the selected criteria


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enverus Energy Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List active drilling rigs in the Permian basin."

**🤖 AI Agent:**
> I've found 15 active rigs in the Permian basin, operated by companies including 'Chevron' and 'Occidental'. Would you like the technical details for rig 'PERM-001'?

---

**👤 You:**
> "Show me production stats for well ID '42-123-45678'."

**🤖 AI Agent:**
> Well ID '42-123-45678' (Eagle Ford #1) is producing 450 BOE/d. The gas-to-oil ratio is 1,200 scf/bbl. Production has remained stable over the last 30 days. Should I pull the historical production trend?

---

**👤 You:**
> "What are the latest energy M&A deals?"

**🤖 AI Agent:**
> I've retrieved 5 recent deals, including the '$2.5B Acquisition of Bakken Assets' by 'Continental Resources' and a '$500M divestiture' in the Eagle Ford. Would you like to see the asset breakdown for the Bakken deal?


## ❓ FAQ

**Q: How do I get an Enverus API Key?**
You need an active Enverus subscription. Log in to your [**Enverus Developer Portal**](https://developer.enverus.com), navigate to your account settings, and you can generate or retrieve your unique **API Key** from there.

**Q: Does the integration cover global basins?**
Yes, Enverus tracks asset activity globally. Availability of specific data for basins like Permian, Bakken, or international fields depends on your subscription level and API permissions.

**Q: Is production data real-time?**
Production data is updated as frequently as reported by operators and regulatory agencies. You can retrieve the latest available telemetry using the get_well_production_telemetry tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/enverus-energy-intelligence](https://vinkius.com/mcp/enverus-energy-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enverus Energy Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enverus-energy-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enverus Energy Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enverus-energy-intelligence": {
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
