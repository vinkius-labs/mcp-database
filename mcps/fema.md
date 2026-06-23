# FEMA MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fema)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access disaster and emergency data via OpenFEMA — track disaster declarations, housing assistance, and hazard mitigation directly through your AI agent.

## Description
Connect to the **OpenFEMA** public database through any AI agent and gain instant access to official data regarding disasters, emergency management, and federal assistance programs.

### What you can do

- **Disaster Tracking** — List official FEMA disaster declarations since 1953 and fetch detailed metadata for specific incidents natively
- **Emergency Orchestration** — List emergency management agencies by state to verify local coordination contacts flawlessly
- **Assistance Analysis** — Query housing assistance program data and individual assistance registrations to analyze recovery efforts natively
- **Grant Inspection** — Access hazard mitigation assistance projects and grant details to monitor community safety investments flawlessly
- **Regional Insights** — List official FEMA regions and web center locations to understand federal jurisdictional boundaries synchronously
- **Public Data Access** — Retrieve raw structured data from the official U.S. Federal Emergency Management Agency API without complex manual exports

### How it works

1. Subscribe to this server
2. Enter your optional OpenFEMA API Key (for higher rate limits)
3. Start querying disaster data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Emergency Responders** — quickly look up disaster history or local agency contacts during planning or operations
- **Policy Analysts** — monitor federal assistance distribution and hazard mitigation trends across specific states
- **Data Researchers** — pull aggregated disaster metrics directly into your AI-powered public safety workflow


## Available Tools (11)
- **get_disaster_applications**: Get statistics on disaster assistance applications
- **get_emergency_agencies**: List emergency management agencies by state
- **get_fema_regions**: List official FEMA regions
- **get_fema_web_centers**: List FEMA web center locations
- **get_hazard_mitigation_grants**: Get data on hazard mitigation assistance projects
- **get_housing_assistance**: Get data regarding FEMA housing assistance programs
- **get_individuals_program**: Get data on individuals and households program registrations
- **get_me**: Get current API status
- **get_public_assistance_applicants**: List applicants for FEMA public assistance
- **get_registration_intake**: Get data from individual and household program registrations
- **list_disaster_declarations**: List recent official FEMA disaster declarations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FEMA** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List recent disaster declarations in Florida."

**🤖 AI Agent:**
> Searching OpenFEMA... I found the latest declarations for Florida, including Hurricane Ian and severe storm events. Would you like to see the breakdown by affected counties?

---

**👤 You:**
> "Get emergency management agency info for California."

**🤖 AI Agent:**
> Retrieving agency data... For California, I've identified Cal OES (Governor's Office of Emergency Services) as the primary state agency. Would you like their headquarters address and contact details?

---

**👤 You:**
> "Show hazard mitigation projects in Texas."

**🤖 AI Agent:**
> Inspecting Hazard Mitigation Assistance projects... I found several active grants in Texas focused on flood control and infrastructure resilience. Shall I list the funding amounts for these projects?


## ❓ FAQ

**Q: Is an API Key required for OpenFEMA?**
No, OpenFEMA data is public. However, using an API Key is recommended for heavy users to ensure higher rate limits and consistent access.

**Q: What types of disasters are included in the data?**
The database includes all incidents resulting in a federal declaration, such as floods, hurricanes, fires, snowstorms, and severe storms.

**Q: How can I filter results by state?**
Use the `filter` parameter with OData syntax, for example: `state eq 'CA'` to retrieve records only for California.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fema](https://vinkius.com/mcp/fema)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FEMA** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fema` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FEMA** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fema": {
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
