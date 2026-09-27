# NYC Open Data Explorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-open-data-explorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Keyless explorer over the 3,000+ datasets of NYC Open Data: catalog search, dataset metadata with column lists, generic SOQL row browsing, grouped stats and row counts — no API key.

## Description
The meta-interface to the city of New York's public data. Instead of one fixed dataset, this MCP lets an agent discover and query the whole NYC Open Data platform (data.cityofnewyork.us) — the same Socrata SODA API the city publishes.

### What you can do
- **Search the catalog** — keyword search over the 3,000+ datasets (id, name, description, update time, monthly views)
- **Inspect a dataset** — full metadata: description, last update, download count and the complete column list
- **Browse any dataset** — generic row query with SOQL filters, column projection, sort, limit and offset
- **Dataset stats** — total row count, optionally filtered, plus top-N values of any column (grouped counts)
- **Row counts** — exact totals for sizing a question before pulling rows

### Notes
- All access is anonymous; no credentials are defined.
- SOQL string literals use double quotes (borough="QUEENS"); date comparisons use ISO "YYYY-MM-DD". Column names must match the dataset exactly — inspect them with get_dataset_info first.
- The ny-* suite also ships purpose-built MCPs for the highest-value dataset families (311, buildings, traffic, crime, food, TLC, parking, climate, citylife).


## Available Tools (5)
- **browse_dataset**: Filters use SOQL: string values must be wrapped in DOUBLE quotes (borough="QUEENS"), date comparisons use ISO "YYYY-MM-DD" (created_date >= "2026-01-01"), and only double-quoted comparisons — no case-insensitive matching. Check the exact column names with get_dataset_info first. Without parameters it returns the newest-looking sample rows; pass order to control the sort.

Query rows of any NYC Open Data dataset with SOQL filters
- **dataset_row_count**: Use it for quick "how big is this dataset" checks; for the breakdown by column use dataset_stats instead.

Exact total row count of a dataset, optionally filtered
- **dataset_stats**: group_by must be an exact column name from get_dataset_info.

Total row count of a dataset, optionally filtered and grouped by a column
- **get_dataset_info**: Use it before browse_dataset to learn the exact column names. The id is the 8-character value returned by search_datasets (format like "erm2-nwe9").

Get the columns, description and update time of one NYC Open Data dataset by id
- **search_datasets**: Returns the dataset id, name, short description and last update time for each match. Use the id with get_dataset_info (columns and details) or browse_dataset (row queries). Start with short keywords like "potholes", "311", "trees" or "taxi".

Search the 3,000+ dataset NYC Open Data catalog by keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Open Data Explorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which NYC datasets are about potholes?"

**🤖 AI Agent:**
> search_datasets("potholes") returns the matching datasets (e.g. DOT Pothole Work Orders, 311 Street Condition requests) with ids and last update; browse one with browse_dataset.

---

**👤 You:**
> "What columns does the 311 service requests dataset have?"

**🤖 AI Agent:**
> get_dataset_info("erm2-nwe9") returns the full column list (unique_key, complaint_type, descriptor, borough, incident_address, latitude, longitude, ...), the dataset description and its last row update.

---

**👤 You:**
> "How big is the 311 dataset and what are the top complaint types?"

**🤖 AI Agent:**
> dataset_row_count("erm2-nwe9") gives the total (22M+ rows); dataset_stats with group_by "complaint_type" returns the most frequent complaint types with counts.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: How do I find the id of a dataset?**
Use search_datasets with a keyword — it queries the platform catalog and returns each match's 8-character id (like "erm2-nwe9"). That id feeds get_dataset_info, browse_dataset, dataset_stats and dataset_row_count.

**Q: Borough values differ across datasets — how do I know the format?**
Formats are dataset-specific: 311 and shootings use UPPERCASE ("QUEENS"), food and sanitation use Title Case ("Queens"), DOT potholes use single-letter codes. Tool descriptions state the expected values, and the errors from a mismatched value are reported verbatim by the platform.

**Q: What size is the catalog?**
The platform catalogs about 3,000 entries: roughly 2,400 standard datasets, plus filtered views, maps and external data sources. search_datasets searches all of them; the ny-* suite MCPs wrap the most-used families with dedicated tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-open-data-explorer](https://vinkius.com/en/ai-agent-connect/nyc-open-data-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Open Data Explorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-open-data-explorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Open Data Explorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-open-data-explorer": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
