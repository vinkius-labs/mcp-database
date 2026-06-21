# OECD Data API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/oecd-data-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access global economic data — audit social and fiscal series via AI.

## Description
Empower your AI agent to orchestrate your entire macroeconomic research and policy auditing workflow with the **OECD Data API**, the authoritative source for global social and economic indicators. By connecting the OECD SDMX-JSON service to your agent, you transform complex statistical searches into a natural conversation. Your agent can instantly retrieve historical datasets, audit regional economic trends, and query specific dataflows without you ever touching a data portal. Whether you are conducting international market research or managing regional policy constraints, your agent acts as a real-time data analyst, ensuring your intelligence is always verified and precise.

### What you can do

- **Dataset Auditing** — Retrieve high-resolution statistical data for thousands of OECD identifiers and maintain a clear view of global economic changes.
- **Indicator Oversight** — Audit historical social and fiscal indicators to understand the longitudinal distribution of economic scale instantly.
- **Dataflow Discovery** — Browse all available dataflows in the OECD catalog to identify relevant thematic markers for your research.
- **Macro Intelligence** — Retrieve unique dataset identifiers and observation metadata to assist in deep-dive archival classification.
- **Operational Monitoring** — Check API status to ensure your economic research workflow is always operational.

### How it works

1. Subscribe to this server
2. No API Key required (OECD REST API is a free and open service)
3. Start managing your economic intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Economists & Policy Analysts** — monitor global trends and retrieve official metadata straight from your workflow.
- **Researchers & Students** — verify statistical data and audit series patterns without manual searching.
- **Financial Journalists** — perform rapid audits of regional indicators and identify relevant economic markers through natural language.
- **Operations Leads** — automate statistical data querying to orchestrate cross-functional research teams smoothly.


## Available Tools
- **check_api_status**: Check if the OECD Data service is operational
- **get_oecd_dataset**: Get specific economic or social data from an OECD dataset ID
- **list_oecd_dataflows**: List all available dataflows and datasets in the OECD catalog


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OECD Data API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get quarterly national accounts (QNA) data from OECD."

**🤖 AI Agent:**
> I've retrieved the QNA dataset! The latest observations show a growth trend of [Value] across member countries. I can provide the full statistical breakdown or specific regional metadata for you.

---

**👤 You:**
> "List all available dataflows in the OECD catalog."

**🤖 AI Agent:**
> I've scanned the OECD dataflow catalog! There are hundreds of series available, including markers for education, health, and fiscal policy. I can help you retrieve a specific dataset ID for any of these thematic markers.

---

**👤 You:**
> "What are the latest observations for the 'CPI' dataset in the OECD?"

**🤖 AI Agent:**
> I've retrieved the CPI observations! The recent data points indicate an inflation trend of [Value] for [Period]. I can assist you with an audit of the comparative metadata across different OECD regions if you'd like.


## ❓ FAQ

**Q: Is an API Key required for OECD Data API?**
No. The OECD REST API is a free and open service. This server works out of the box without any static credentials required.

**Q: What format is the data returned in?**
The API returns data in the SDMX-JSON format, which includes detailed observations and metadata for economic series.

**Q: Can the agent list multiple datasets?**
Yes. The `list_oecd_dataflows` tool retrieves the complete list of available dataflows and datasets from the OECD catalog.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/oecd-data-api](https://vinkius.com/mcp/oecd-data-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OECD Data API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `oecd-data-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OECD Data API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "oecd-data-api": {
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
