# Dados.gov.pt Open Data MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/dadosgovpt-open-data)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Portugal's national open data catalog: search 20,000+ datasets from ministries, municipalities and public bodies, inspect resources, preview CSV/JSON data and browse publishing organizations — all zero-auth.

## Description
The **official Portuguese public sector open data portal** (dados.gov.pt) as a single MCP server.

### What you can do
- **Discover** — full-text search across 20,000+ open datasets covering health, tourism, finance, municipalities, environment and more
- **Inspect** — complete dataset metadata: resources, formats, licenses, spatial/temporal coverage, quality metrics
- **Preview data** — fetch actual CSV/JSON resource content through the portal's proxy, with size-capped previews
- **Browse publishers** — search ministries, municipalities (Câmara Municipal), institutes and agencies; inspect each organization's profile
- **Curated picks** — list the portal's featured datasets

### Who is this for?
Analysts, journalists, researchers and AI agents that need authoritative Portuguese public data: statistics, budgets, health indicators, municipal transparency and more — all published under open licenses, no authentication required.


## Available Tools (8)
- **list_featured_datasets**: gov.pt team as featured. Useful for discovery and inspiration.

List featured/highlighted open data datasets
- **search_datasets**: gov.pt. Returns id, title, slug, organization, tags, formats and last update. Use page to navigate results (never fetch all pages).

Search open data datasets from the Portuguese public sector (20,000+ datasets)
- **get_dataset**: Get full metadata of a dataset (resources, license, coverage, quality)
- **get_resource**: gov.pt proxy and returns a text preview. Use get_dataset first to find resource ids. Large files are truncated to max_chars characters.

Fetch the actual data of a dataset resource (CSV/JSON preview)
- **search_by_tag**: Returns id, title, slug, organization and formats. Use page to navigate.

Search datasets by tag (e.g. "turismo", "saude")
- **search_by_format**: The format is case-sensitive and lowercase (e.g. "csv", "json", "shp", "xlsx") — note that many publishers do not tag formats, so combine with search_datasets for full coverage.

Search datasets offering a specific file format (csv, json, xlsx...)
- **search_organizations**: gov.pt organizations by name. Returns id, name, acronym, description and dataset counts. Use the id in get_organization.

Search public bodies publishing open data (ministries, municipalities...)
- **get_organization**: Combine with search_datasets (query=org name) to list its datasets.

Get full profile of a publishing organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dados.gov.pt Open Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find open data about tourism in Portugal and tell me what formats are available"

**🤖 AI Agent:**
> 🇵🇹 **Tourism datasets on dados.gov.pt**

39 datasets found. Highlights:
- **Dormidas e proveitos na alojamento** (INE) — monthly hotel stays & revenue, CSV + JSON
- **PME Turismo de Portugal** — funding beneficiaries, CSV
- **Proveitos do turismo receiver** — regional revenue series

Most offer CSV; INE-sourced datasets also expose JSON indicator APIs. I can preview any of them next.

---

**👤 You:**
> "Which municipalities publish open data and how much have they published?"

**🤖 AI Agent:**
> 🏛️ **Municipal open data publishers**

Top publishers found:
- **Câmara Municipal de Lisboa** — dozens of datasets (mobility, equipment, environment)
- **Câmara Municipal do Porto** — urban data portal mirrors
- **Cascais**, **Aveiro**, **Braga** — growing catalogs

I can drill into any municipality's profile or list its datasets next.

---

**👤 You:**
> "Preview the first rows of the health indicators dataset about pharmacists per 1000 inhabitants"

**🤖 AI Agent:**
> 💊 **Pharmacists per 1000 inhabitants (INE)**

Preview of the JSON resource:
```
IndicadorCod: 0014855
Distribuição: Local de trabalho (NUTS - 2024)
Periodicidade: Anual
```
First data rows show values by NUTS region with latest year available. The full file is ~1MB of JSON — I can pull more rows or filter by region if you want.


## ❓ FAQ

**Q: Do I need an API key or registration?**
No. dados.gov.pt is a fully open portal — every tool in this MCP works without any authentication or account.

**Q: Can I download the actual data files?**
The get_resource tool previews a resource's content through the portal's proxy (truncated to keep responses manageable). For very large files, use the resource URL from get_dataset to fetch data in chunks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/dadosgovpt-open-data](https://vinkius.com/en/ai-agent-connect/dadosgovpt-open-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dados.gov.pt Open Data** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dadosgovpt-open-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dados.gov.pt Open Data** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dadosgovpt-open-data": {
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
