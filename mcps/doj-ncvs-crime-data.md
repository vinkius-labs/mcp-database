# DOJ NCVS Crime Data MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/doj-ncvs-crime-data)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data](../categories/data.md)

Access US crime statistics — audit victimization data and safety via AI.

## Description
Empower your AI agent to orchestrate your entire public safety research workflow with **DOJ NCVS Crime Data**, the authoritative source for United States victimization statistics. By connecting the DOJ API to your agent, you transform complex crime data lookups into a natural conversation. Your agent can instantly retrieve personal and household victimization rates, audit historical crime trends, and identify regional safety markers without you ever touching a technical data portal. Whether you are conducting sociological research or monitoring community safety, your agent acts as a real-time safety analyst, ensuring your intelligence is always grounded in official, government-verified data.

### What you can do

- **Personal Auditing** — Retrieve statistics on personal victimization, including assault and theft, to maintain a clear view of safety trends.
- **Household Oversight** — Audit household-level crime data, such as burglary and motor vehicle theft, to understand residential security.
- **Temporal Intelligence** — Query crime statistics for specific years to audit past and current public safety trends instantly.
- **Regional Discovery** — Retrieve crime data for specific US regions to understand geographic distributions of victimization.
- **Attribute Intelligence** — List all available categories and attributes in the NCVS catalog to identify relevant safety markers.

### How it works

1. Subscribe to this server
2. No API Key required (DOJ NCVS is a public and free service)
3. Start managing your public safety intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Criminologists & Researchers** — monitor victimization patterns and retrieve official metadata straight from your workflow.
- **Journalists** — verify crime trends and audit public safety records without manual database exports.
- **Policy Analysts** — perform rapid audits of crime markers and identify regional clusters through natural language.
- **Operations Leads** — automate public safety data querying to orchestrate cross-functional community teams smoothly.


## Available Tools (6)
- **check_api_status**: Check if the DOJ NCVS API is operational
- **get_crime_by_region**: Get crime statistics for a specific US region
- **get_crime_by_year**: Get all crime statistics for a specific year
- **get_household_victimization**: Get household victimization statistics from NCVS
- **get_personal_victimization**: Get personal victimization statistics from NCVS
- **list_crime_attributes**: List available attributes and categories in the NCVS database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DOJ NCVS Crime Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What were the personal victimization rates in the US for 2022?"

**🤖 AI Agent:**
> I've retrieved the 2022 statistics. The personal victimization rate was approximately 23.5 per 1,000 persons. This includes assault and theft data. Would you like the breakdown by offense type?

---

**👤 You:**
> "Show household crime data for the 'South' region."

**🤖 AI Agent:**
> I've retrieved the household victimization data for the South region. Notable trends include burglary and property theft rates. Would you like to compare this with national averages?

---

**👤 You:**
> "List all categories in the NCVS database."

**🤖 AI Agent:**
> I've scanned the NCVS catalog. It includes over 50 attributes, from 'Offense Type' and 'Victim Demographic' to 'Reporting to Police'. I can help you query any of these markers.


## ❓ FAQ

**Q: Is an API Key required for DOJ Crime Data?**
No. The DOJ NCVS API is a public and free service. This server works out of the box without any static credentials required.

**Q: What types of crime are included in the statistics?**
The NCVS includes data on personal crimes (assault, theft) and household crimes (burglary, motor vehicle theft). Use the `list_crime_attributes` tool to see the full catalog.

**Q: Is the data national or state-level?**
The API provides national-level victimization data, often categorized by broad geographic regions (e.g., South, West) and population sizes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/doj-ncvs-crime-data](https://vinkius.com/mcp/doj-ncvs-crime-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DOJ NCVS Crime Data** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `doj-ncvs-crime-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DOJ NCVS Crime Data** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "doj-ncvs-crime-data": {
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
