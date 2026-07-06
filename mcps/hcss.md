# HCSS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hcss)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Automate heavy construction management via HCSS — manage jobs, timecards, estimates, and equipment telematics directly from any AI agent.

## Description
Connect your **HCSS** platform to any AI agent and take full control of your heavy construction workflows, from estimating to field data and equipment tracking, through natural conversation.

### What you can do

- **Field Data Management** — List construction jobs and retrieve timecard data from HeavyJob to monitor site progress.
- **Estimating Insights** — Access bidding estimates and bid items from HeavyBid to stay aligned with project budgets.
- **Equipment Telematics** — Monitor your fleet with real-time GPS locations and latest meter readings (odometer/hours).
- **Resource Coordination** — List employees and business units defined across the HCSS ecosystem.
- **Pre-Construction Tracking** — Browse active pre-con projects and project lifecycles.
- **Operational Efficiency** — Use AI to identify equipment utilization trends or job cost variances in seconds.

### How it works

1. Subscribe to this server
2. Enter your HCSS Client ID, Client Secret, and API Key (Subscription Key)
3. Start managing your construction projects from Claude, Cursor, or any MCP-compatible client

No more manual exporting of field reports or logging into multiple portals. Your AI assistant acts as a dedicated Project Engineer or Fleet Manager.

### Who is this for?

- **Project Managers** — instantly retrieve job costs and timecard statuses straight from the field.
- **Fleet Managers** — check equipment locations and maintenance needs without digging through telematics screens.
- **Estimators** — verify bid item details and estimate progress during high-pressure bidding cycles.


## Available Tools (11)
- **list_cost_codes**: List cost codes defined in the system
- **list_employees**: List all employees synced in HCSS
- **list_equipment**: List all tracked equipment/fleet from Telematics
- **list_estimates**: List bidding estimates from HeavyBid
- **list_jobs**: List all construction jobs/projects
- **list_precon_projects**: List active pre-construction projects
- **list_timecards**: List timecards from HeavyJob
- **get_bid_items**: List bid items for a specific estimate
- **get_equipment_location**: Get current GPS coordinates for a specific piece of equipment
- **get_equipment_meters**: Get latest meter readings (odometer/hours) for equipment
- **list_business_units**: List all business units in HCSS


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HCSS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active construction jobs."

**🤖 AI Agent:**
> I've retrieved your jobs. You have 5 active projects, including 'Highway 101 Expansion' (ID: 5501), 'Downtown Bridge Repair' (ID: 5505), and 'Industrial Park Phase 2'. Which one would you like to see timecard summaries for?

---

**👤 You:**
> "Show the current location of Excavator ID EX-992."

**🤖 AI Agent:**
> Accessing telematics... Excavator EX-992 is currently located at (29.7604, -95.3698), which is near the 'Highway 101' job site. The engine was last reported running 2 hours ago. Should I check the fuel level or meter readings?

---

**👤 You:**
> "What are the bid items for estimate ID 2024-001?"

**🤖 AI Agent:**
> Retrieving HeavyBid data... Estimate 2024-001 includes 12 bid items, such as 'Site Clearing', 'Foundation Piling', and 'Asphalt Paving'. Would you like to see the assigned quantities and unit prices for these items?


## ❓ FAQ

**Q: How do I obtain my HCSS API credentials?**
You must request API access through the **HCSS Developer Portal** (developer.hcssapps.com). Once approved, you will receive your Client ID, Client Secret, and Ocp-Apim-Subscription-Key.

**Q: Can I see the real-time location of my equipment?**
Yes! Use the `get_equipment_location` tool with the unique equipment ID. It will return the latest GPS coordinates recorded by the Telematics system.

**Q: Does this integration cover both HeavyJob and HeavyBid?**
Yes, this MCP server includes tools for both modules, allowing you to access timecard data from HeavyJob and estimate/bid data from HeavyBid in a single interface.

**Q: Is the integration secure for construction data?**
Absolutely. The integration uses industry-standard OAuth 2.0 Client Credentials flow and HTTPS. Your credentials are encrypted and stored securely within the Vinkius Cloud infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hcss](https://vinkius.com/mcp/hcss)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HCSS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hcss` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HCSS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hcss": {
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
