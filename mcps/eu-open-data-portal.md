# EU Open Data Portal MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/eu-open-data-portal)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Search 1.9M+ open datasets from 36 European countries in data.europa.eu — the official EU portal: full-text search, per-country and format filters, High-Value Datasets (HVD) finder and full dataset details with download links — zero auth.

## Description
The **European Open Data Portal (data.europa.eu)** as a single MCP server — the official EU portal aggregating open data from all member states and neighbouring countries.

### What you can do
- **Full-text search across 1.9M+ datasets** — titles, descriptions, publishers, keywords, with pagination
- **Country-focused search** — slice any query by one of 36 country codes (national portals are all harvested)
- **Format-aware search** — keep only datasets with CSV/JSON/GeoJSON/XML distributions, so agents get data they can actually parse
- **High-Value Datasets (HVD)** — find the datasets EU regulation 2023/138 obliges member states to publish free, machine-readable and via APIs: geospatial, earth observation, meteorological, statistics, company registries and mobility
- **Full dataset details** — every distribution with direct download URLs, licences, contact points, temporal/spatial coverage and data.europa.eu quality scores
- **Catalogue browser** — see the national and thematic sources behind every dataset

### Why data.europa.eu
This is the single entry point to Europe's public data infrastructure: national portals (dados.gov.pt, data.gouv.fr, govdata.de...), EU institutions (Eurostat, EEA, ECA) and the mandated High-Value Datasets. An agent that can search it can ground market research, journalism, policy analysis and product development in official public data — no API key, no registration.

### Typical workflows
- Market research: company registries and statistics per country (HVD category)
- Environment/energy analysis: air quality, earth observation and meteorological HVDs
- Mobility apps: GTFS transport feeds and geospatial HVDs
- Due diligence: verify publishers and licences before reuse


## Available Tools (8)
- **get_dataset_details**: Unlike the search rows, this returns every distribution (file) with accessUrl/downloadUrl, format and licence, plus contact points, temporal/spatial coverage and data.europa.eu quality scores (accessible/known licences etc.). Use it as the step right before actually downloading a dataset.

Full details for one dataset: all distributions with direct download URLs, formats, licence, contacts and quality measurements
- **find_high_value_datasets**: High-Value Datasets are the six categories the EU considers most valuable for reuse: geospatial, earth observation & environment, meteorological, statistics, companies & company ownership, and mobility — each with special licensing obligations (free, machine-readable, APIs). Use when you want the EU's curated best data for market research, apps or products. Query is MANDATORY.

Find EU "High-Value Datasets" (HVD) — the datasets the EU mandates member states to provide for free and via APIs
- **find_hvd_in_country**: Great for "what is Portugal legally required to open up?" style questions. Query is MANDATORY.

High-Value Datasets from one specific European country (e.g. "pt" Portugal, "de" Germany) — curated, API-accessible data
- **search_datasets_by_country**: Use for country-specific questions: national statistics, government spending, environment, transport. Note the portal aggregates national portals, so coverage mirrors what each country publishes. Query is MANDATORY.

Search all open datasets — not only HVDs — from one specific European country
- **search_datasets_by_format**: g. "csv", "json", "geojson", "xml", "parquet", "shp"). Ideal when an agent needs data it can parse directly instead of PDFs. Query is MANDATORY.

Search datasets and see/download only machine-readable formats (CSV, JSON, XML, GeoJSON...)
- **list_catalogues**: europa.eu — typically one per country's national open data portal plus thematic sources (EEA, Eurostat, EDP...). Useful for understanding data provenance: a dataset's "catalogue" field links back to one of these. Pass a keyword to try filtering by name substring.

Browse the national and thematic catalogues harvested by the portal (one catalogue per source: national portals, EEA, Eurostat...)
- **get_portal_reference**: Read it before country/HVD workflows if unsure.

Reference: what data.europa.eu is, HVD categories, EU country codes and usage tips for the other tools
- **search_datasets**: europa.eu, official EU portal aggregating national portals). Each row has: id, title, trimmed description, country, publisher, categories, keywords, dates and the landing page URL. Query is MANDATORY. Combine topic + geography keywords, e.g. "air quality berlin", "tourism statistics portugal", "public transport gtfs". Too many hits? Narrow with search_datasets_by_country or add more specific keywords. Take dataset ids into get_dataset_details for download links.

Search 1.9M+ open datasets from 36 European countries in the official data.europa.eu portal — titles, publishers, countries, keywords and download landing pages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EU Open Data Portal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find open data about air quality in Portugal that I can download as CSV"

**🤖 AI Agent:**
> 📊 **Air quality data in Portugal (CSV)**

From data.europa.eu:
1. **QualAr — Air Quality Index** (APA, PT) — daily per-station index, CSV distributions
2. **EEA AirBase** — harmonised European measurements incl. PT stations, CSV/JSON

Take the dataset ids and I'll pull get_dataset_details for the direct download URLs, licences and update frequency.

---

**👤 You:**
> "Which High-Value Datasets must Germany provide? I need company registry data for market research"

**🤖 AI Agent:**
> 🏛️ **Germany's High-Value Datasets — companies category**

Under Regulation 2023/138, company registries are a mandatory HVD category. From data.europa.eu (filtered: country=de, HVD):
- **Unternehmensregister** — official German company register distributions
- **North Data** sample datasets — structured company ownership data

These are free and machine-readable by law. I can pull full details (download URLs, licences) for whichever you pick.


## ❓ FAQ

**Q: Do I need an API key, and is the data free to reuse?**
No key needed — the portal's search API is fully public. Reuse conditions belong to each dataset: most open data is CC-BY or similar, but licences vary per source, so always check the licence field in get_dataset_details before republishing. High-Value Datasets are guaranteed free and machine-readable by EU regulation.

**Q: Why does country/format filtering sometimes return fewer rows than requested?**
The portal's public search API does not expose server-side country/format facets, so those tools fetch a larger page and filter client-side; when a page contains few matches, results can be sparse — advance the page or refine keywords. The underlying data is all there; it is a pagination artifact, not missing data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/eu-open-data-portal](https://vinkius.com/en/ai-agent-connect/eu-open-data-portal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EU Open Data Portal** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `eu-open-data-portal` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EU Open Data Portal** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eu-open-data-portal": {
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
