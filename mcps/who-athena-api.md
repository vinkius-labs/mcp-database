# WHO Athena API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/who-athena-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access global health data — audit indicators and trends via AI.

## Description
Empower your AI agent to orchestrate your entire public health research and policy auditing workflow with the **WHO Athena API**, the authoritative source for global health indicators from the World Health Organization. By connecting the WHO GHO service to your agent, you transform complex medical searches into a natural conversation. Your agent can instantly retrieve historical datasets, audit regional health trends, and query specific indicator codes without you ever touching a health portal. Whether you are conducting epidemiological research or managing regional policy constraints, your agent acts as a real-time health analyst, ensuring your intelligence is always verified and precise.

### What you can do

- **Indicator Auditing** — Retrieve high-resolution statistical data for thousands of WHO health identifiers and maintain a clear view of global health changes.
- **Trend Oversight** — Audit historical health statistics to understand the longitudinal distribution of medical scale instantly.
- **Dimension Discovery** — Browse all available observation dimensions like 'country' or 'year' to maintain strict organizational control over your research.
- **Medical Intelligence** — Retrieve unique indicator codes and observation metadata to assist in deep-dive archival classification.
- **Operational Monitoring** — Check API status to ensure your health research workflow is always operational.

### How it works

1. Subscribe to this server
2. No API Key required (WHO GHO API is a free and open service)
3. Start managing your health intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Health Analysts & Policy Makers** — monitor global trends and retrieve official metadata straight from your workflow.
- **Epidemiologists & Researchers** — verify statistical data and audit series patterns without manual searching.
- **Medical Journalists** — perform rapid audits of regional indicators and identify relevant health patterns through natural language.
- **Operations Leads** — automate health data querying to orchestrate cross-functional research teams smoothly.


## Available Tools (4)
- **check_api_status**: Check if the WHO GHO Athena service is operational
- **get_health_indicator_data**: Get data for a specific WHO health indicator code
- **list_health_dimensions**: List all observation dimensions (e.g., country, year) available
- **list_health_indicators**: List all health indicators available in the WHO GHO database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WHO Athena API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get data for 'Life expectancy at birth' (WHOSIS_000001) using WHO Athena."

**🤖 AI Agent:**
> I've retrieved the data for life expectancy! The latest observations show a global average of [Value] years. I can provide the breakdown by country or region metadata for you.

---

**👤 You:**
> "List all health indicators available in the WHO catalog."

**🤖 AI Agent:**
> I've scanned the WHO indicator catalog! There are thousands of series available, including markers for infectious diseases, child mortality, and health systems. I can help you find a specific code for your research.

---

**👤 You:**
> "What are the latest observations for 'Child mortality rate'?"

**🤖 AI Agent:**
> I've retrieved the observations for child mortality! The recent data points indicate a trend of [Value] per 1000 live births. I can assist you with an audit of the comparative metadata across different WHO regions if you'd like.


## ❓ FAQ

**Q: Is an API Key required for WHO Athena API?**
No. The WHO Global Health Observatory API is a free and open service. This server works out of the box without any static credentials required.

**Q: What format is the data returned in?**
The API returns detailed health indicator data including numeric values, spatial dimensions (countries), and time dimensions (years).

**Q: Can I filter by indicator code?**
Yes. Use the `get_health_indicator_data` tool and provide the WHO indicator code (e.g., 'WHOSIS_000001' for life expectancy).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/who-athena-api](https://vinkius.com/mcp/who-athena-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WHO Athena API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `who-athena-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WHO Athena API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "who-athena-api": {
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
