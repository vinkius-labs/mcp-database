# GovCon API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/govcon-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Manage government contracts — audit opportunities and agencies via AI.

## Description
Empower your AI agent to orchestrate your entire business development and government contracting workflow with the **GovCon API**, the authoritative source for procurement data. By connecting the GovCon API to your agent, you transform complex contract searches into a natural conversation. Your agent can instantly search for active opportunities, audit agency distributions, and retrieve detailed procurement metadata without you ever touching a government portal. Whether you are conducting market research or managing regional bid constraints, your agent acts as a real-time procurement consultant, ensuring your data is always verified and precise.

### What you can do

- **Contract Auditing** — Search for thousands of government contracts and procurement opportunities by keyword or agency and maintain a clear view of market distribution.
- **Agency Oversight** — Audit all registered government agencies in the catalog to understand the organizational reach of public sector procurement instantly.
- **Opportunity Discovery** — Retrieve high-resolution details for specific opportunity IDs to assist in deep-dive classification.
- **Metadata Intelligence** — Retrieve unique identifiers and amount markers for any government contract to assist in deep-dive fiscal analysis.
- **Operational Monitoring** — Check API status to ensure your procurement research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your GovCon API Key
3. Start managing your procurement intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Government Contractors** — monitor opportunity timelines and retrieve official metadata straight from your workflow.
- **Market Researchers** — verify agency patterns and audit procurement distributions without manual searching.
- **Business Development Leads** — perform rapid audits of contract markers and identify relevant lead patterns through natural language.
- **Operations Leads** — automate procurement data querying to orchestrate cross-functional business teams smoothly.


## Available Tools
- **check_api_status**: Check if the GovCon service is operational
- **get_procurement_details**: Get full details for a specific government opportunity by ID
- **list_government_agencies**: List all government agencies registered in the GovCon database
- **search_government_contracts**: Search for government contracts and procurement opportunities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GovCon API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for government contracts related to 'cybersecurity' using GovCon."

**🤖 AI Agent:**
> I've retrieved several cybersecurity contracts! Notable entries include requirements for network monitoring and system audits. Would you like the full details for the top matches or the agency metadata?

---

**👤 You:**
> "Show details for opportunity ID '12345'."

**🤖 AI Agent:**
> I've retrieved the details for opportunity 12345! It is identified as a [Title] for [Agency]. The estimated value is [Amount]. I can assist you with the full procurement metadata for this site if you'd like.

---

**👤 You:**
> "List all government agencies available in GovCon."

**🤖 AI Agent:**
> I've scanned the agency catalog from GovCon! There are over 50 agencies listed, including the DOD, NASA, and local departments. I can provide the unique ID and distribution for each of these platforms to assist in your market audit.


## ❓ FAQ

**Q: How do I find my GovCon API Key?**
Log in to your [**GovCon account**](https://govconapi.com/), and you will find your API Key in your dashboard. Copy and paste it below.

**Q: Does it support multiple agencies?**
Yes. GovCon aggregates procurement data across various federal and local government agencies.

**Q: Can the agent show award amounts?**
Yes. Every contract record retrieved by your agent includes metadata on the award amount where available.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/govcon-api](https://vinkius.com/mcp/govcon-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GovCon API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `govcon-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GovCon API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "govcon-api": {
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
