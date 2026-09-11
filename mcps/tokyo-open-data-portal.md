# Tokyo Open Data Portal MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tokyo-open-data-portal)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Tokyo Metropolitan Government's official open data portal: 9,600+ datasets on disaster prevention, tourism, transport (Toei subway), health, environment and the city budget — searchable with pagination, keyless.

## Description
The **official open data catalog of the Tokyo Metropolitan Government** as a single MCP server — one of the largest municipal open data portals in the world.

### What you can do
- **Search 9,600+ datasets** — disaster prevention (433), daily life (1,149), health (527), education (827), environment (616), tourism (207), culture (471), infrastructure (808), industry (711), digital tech (95), sports (116)
- **Inspect full metadata** — publisher bureau, license, update frequency and every downloadable resource (CSV, XLSX, GeoJSON...) with direct URLs
- **Preview raw data** — fetch the first rows of a resource before deeper analysis
- **Browse by bureau** — explore entire catalogues of each Tokyo government office (General Affairs alone publishes 2,178 datasets)

### What lives here
Real-time-adjacent civic data: earthquake and flood risk maps, radiation measurements, Toei transport stats, COVID-era health data, electricity usage, population by ward, tourism statistics, cherry-blossom and festival data, Tokyo budget documents — the data behind the world's largest metropolis.

### Who is this for?
Urban researchers, Japan analysts, journalists, real-estate and tourism analysts, civic-tech builders and AI agents that need authoritative Tokyo city data.


## Available Tools (5)
- **get_dataset**: Use ids/slugs from search_datasets (e.g. t000018d0000000001).

Get full metadata of a Tokyo open dataset: description, publisher, and all downloadable resources
- **search_datasets**: data.metro.tokyo.lg.jp. IMPORTANT: query terms go against the TITLE and are Japanese (e.g. 観光 tourism, 防災 disaster prevention, 電力 power, コロナ covid). Filter with group (e.g. c023 観光, c015 防災 — see list_categories) and format (e.g. CSV, XLSX). Paginate with page/page_size — never fetch all pages.

Search the 9,600+ open datasets of the Tokyo Metropolitan Government (disaster, tourism, transport, health, environment...)
- **preview_resource**: Take resource URLs from get_dataset. Best for CSV/JSON; binary formats return limited bytes. Great for inspecting actual rows before deeper analysis.

Preview the raw content of a dataset resource (CSV/XLSX/JSON first rows)
- **list_categories**: Use group ids in search_datasets.

List the 12 thematic categories of the Tokyo open data portal (disaster, tourism, health...)
- **list_organizations**: g. 総務局 General Affairs (2178 datasets), 交通局 Transportation Bureau (Toei subway/bus), 環境局 Environment, etc. Useful to explore a bureau's entire output via search_datasets with its name.

List the Tokyo government bureaus publishing open data (with dataset counts)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tokyo Open Data Portal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find Tokyo datasets about tourism and tell me what's available"

**🤖 AI Agent:**
> 🗼 **Tourism datasets in Tokyo's portal (group c023)**

207 datasets, top hits for 観光:
- **交通局の概要** (Transportation Bureau overview) — Toei subway/bus ridership, CSV
- **観光客数等の実態調査** — visitor count surveys by area
- Hotel/lodging statistics by ward

Most are CSV/XLSX. Want a preview of the visitor survey rows?

---

**👤 You:**
> "What disaster prevention data does Tokyo publish?"

**🤖 AI Agent:**
> 🌊 **Disaster prevention (防災) — 433 datasets**

Highlights:
- Earthquake hazard maps by ward (GeoJSON)
- Flood risk zones for the Arakawa/Tama rivers
- Radiation monitoring measurements
- Emergency shelter locations (CSV)

Critical for any Japan-safety application. I can preview the shelter list or extract GeoJSON for a specific ward.

---

**👤 You:**
> "Which Tokyo bureau publishes the most data?"

**🤖 AI Agent:**
> 🏛️ **Top publishers (organization_list)**

1. 総務局 (General Affairs) — 2,178 datasets: population, statistics, finances
2. 交通局 (Transportation) — Toei subway & bus data
3. 環境局 (Environment) — air quality, energy

General Affairs dominates because it aggregates city-wide statistics. Want me to list its datasets?


## ❓ FAQ

**Q: Do I need an API key or registration?**
No. The portal is a standard CKAN catalog with a fully public API — search, metadata, categories and organizations all work without authentication.

**Q: Why must search terms be in Japanese?**
Dataset titles are published in Japanese; the Solr index matches title: term queries, and English terms like "tourism" match nothing. Use Japanese keywords (観光, 防災, 人口) or browse by category/organization instead. The list_categories tool includes the English meaning of each category.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tokyo-open-data-portal](https://vinkius.com/en/ai-agent-connect/tokyo-open-data-portal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tokyo Open Data Portal** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tokyo-open-data-portal` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tokyo Open Data Portal** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tokyo-open-data-portal": {
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
