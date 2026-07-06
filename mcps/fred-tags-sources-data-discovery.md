# FRED Tags & Sources — Data Discovery MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fred-tags-sources-data-discovery)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Discover FRED series through intelligent tagging: search tags like 'gdp', 'inflation', 'monthly', combine multiple tags to find exactly the right series, and explore all 107 official data sources from BLS to the Census Bureau.

## Description
The discovery layer for FRED. Tags & Sources helps your AI agent find exactly the right series by filtering through FRED's comprehensive tagging system.

### What you can do
- **Search Tags** — Browse geographic (usa, europe), topic (gdp, inflation), source (bls, bea), and frequency (monthly, quarterly) tags
- **Tag Combinations** — Find series matching ALL specified tags (e.g., usa + gdp + quarterly) while excluding others
- **Data Sources** — List all 107 organizations contributing data: BLS, BEA, Federal Reserve Board, Census Bureau, Treasury, IMF, and more

### Who is this for?
Researchers exploring FRED's catalog, data engineers building automated pipelines, and AI agents that need precise series discovery beyond simple keyword search.


## Available Tools (3)
- **list_sources**: List all FRED data sources
- **search_tags**: Search by text or get all tags. Tags include geographic (usa, europe), topic (gdp, inflation), source (bls, bea), and frequency (monthly, quarterly) labels.

Search or browse FRED tags
- **get_series_by_tags**: Powerful for discovering related series. Example: tag_names="usa;gdp" returns all US GDP series. Combine with exclude_tag_names to refine.

Get FRED series matching specific tags


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FRED Tags & Sources — Data Discovery** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all monthly U.S. GDP-related series"

**🤖 AI Agent:**
> 🏷 **Tags: usa + gdp + monthly**

Found 47 matching series:
1. MRTSSM44X72USS — Retail Sales
2. TOTALSA — Vehicle Sales
3. INDPRO — Industrial Production
4. TSIFRGHT — Transportation Index
...

All are monthly U.S. GDP-component indicators.

---

**👤 You:**
> "List all data sources that contribute to FRED"

**🤖 AI Agent:**
> 🏛 **FRED Data Sources (107 total)**

1. Bureau of Labor Statistics (BLS)
2. Bureau of Economic Analysis (BEA)
3. Board of Governors of the Federal Reserve
4. U.S. Census Bureau
5. U.S. Department of the Treasury
6. International Monetary Fund (IMF)
7. World Bank
8. OECD
...

107 official sources spanning U.S. and international organizations.

---

**👤 You:**
> "What tags are most popular on FRED?"

**🤖 AI Agent:**
> 🏷 **Top FRED Tags by Series Count**

1. `usa` — 245K series
2. `monthly` — 178K series
3. `annual` — 156K series
4. `nsa` (not seasonally adjusted) — 142K
5. `county` — 98K series
6. `quarterly` — 67K series
7. `sa` (seasonally adjusted) — 54K
8. `gdp` — 12K series


## ❓ FAQ

**Q: What is the difference between tags and categories?**
Categories are a strict hierarchy (one parent, many children). Tags are flat labels — each series can have many tags across dimensions: geography (usa), frequency (monthly), topic (gdp), source (bls). Combine tags for powerful cross-dimensional filtering.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fred-tags-sources-data-discovery](https://vinkius.com/mcp/fred-tags-sources-data-discovery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FRED Tags & Sources — Data Discovery** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fred-tags-sources-data-discovery` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FRED Tags & Sources — Data Discovery** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fred-tags-sources-data-discovery": {
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
