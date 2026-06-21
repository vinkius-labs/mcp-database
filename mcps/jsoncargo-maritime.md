# JSONCargo Maritime MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jsoncargo-maritime)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Track global vessels — audit voyages and ports via AI.

## Description
Empower your AI agent to orchestrate your entire maritime research and vessel auditing workflow with **JSONCargo Maritime**, the comprehensive source for real-time shipping data. By connecting JSONCargo to your agent, you transform complex logistics searches into a natural conversation. Your agent can instantly search for vessels, audit current voyage statuses, and retrieve detailed port metadata without you ever touching a maritime portal. Whether you are conducting supply chain research or monitoring regional trade constraints, your agent acts as a real-time maritime consultant, ensuring your data is always verified and precise.

### What you can do

- **Vessel Auditing** — Search for thousands of maritime vessels by name or IMO number and retrieve detailed metadata, including flags and types.
- **Voyage Oversight** — Audit the current status and position of vessels to understand the temporal distribution of maritime logistics instantly.
- **Port Discovery** — Browse global ports and their location codes (LOCODEs) to maintain strict organizational control over trade routes.
- **Logistics Intelligence** — Retrieve unique vessel identifiers to assist in deep-dive supply chain classification.
- **Operational Monitoring** — Check API status to ensure your maritime research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your JSONCargo API Key
3. Start managing your maritime intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Supply Chain Analysts** — monitor vessel timelines and retrieve arrival metadata straight from your workflow.
- **Logistics Planners** — verify port locations and audit shipping patterns without manual searching.
- **Trade Researchers** — perform rapid audits of vessel metadata and identify relevant logistics markers through natural language.
- **Operations Leads** — automate maritime data querying to orchestrate cross-functional shipping teams smoothly.


## Available Tools
- **check_api_status**: Check if the JSONCargo service is operational
- **get_current_voyage_details**: Get full metadata for the current voyage of a specific vessel ID
- **list_maritime_ports**: List global ports registered in the JSONCargo database
- **search_maritime_vessels**: Search for maritime vessels by name or IMO number


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JSONCargo Maritime** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for vessel 'Ever Given' using JSONCargo."

**🤖 AI Agent:**
> I've retrieved the details for Ever Given! It is a Container Ship with IMO number 9811000. Would you like the current voyage metadata or the vessel's flag information?

---

**👤 You:**
> "What is the current voyage status for vessel ID 'VES-123'?"

**🤖 AI Agent:**
> I've identified the current voyage for VES-123! It is currently identified as 'En Route' from Singapore to Rotterdam. The current position was updated [Time] ago. I can provide the full track metadata if you'd like.

---

**👤 You:**
> "List all maritime ports in 'Netherlands'."

**🤖 AI Agent:**
> I've retrieved the port catalog for the Netherlands! Notable entries include Rotterdam (NLRTM) and Amsterdam (NLAMS). I can provide the full LOCODE and terminal metadata for each of these sites.


## ❓ FAQ

**Q: How do I find my JSONCargo API Key?**
Log in to your [**JSONCargo account**](https://api.jsoncargo.com/), navigate to your dashboard, and you will find your API Key in the 'Access Tokens' section. Copy and paste it below.

**Q: What vessel identifiers are supported?**
The API supports searching by vessel name, IMO number, and unique JSONCargo identifiers.

**Q: Does it support real-time positions?**
Yes. The `get_current_voyage_details` tool retrieves the most recent position and status metadata for active vessels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jsoncargo-maritime](https://vinkius.com/mcp/jsoncargo-maritime)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JSONCargo Maritime** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `jsoncargo-maritime` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JSONCargo Maritime** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jsoncargo-maritime": {
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
