# Eurostat Discovery — Dataset Catalog Explorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eurostat-discovery-dataset-catalog-explorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Explore Eurostat's catalog of 7,000+ official datasets: search by keyword, inspect dataset dimensions and code lists, and query any dataset with flexible filters — the master key to all European Union statistics.

## Description
The master key to all EU statistics. Discovery lets your AI agent explore, understand, and query any Eurostat dataset.

### What you can do
- **Search** — Find datasets by keyword across 7,000+ Eurostat databases
- **Metadata** — Inspect dimensions, code lists, and frequencies for any dataset
- **Generic Query** — Query any dataset with flexible country and time filters

### Who is this for?
Data explorers, researchers discovering what EU data exists, and AI agents that need to dynamically find and query European statistics.


## Available Tools (3)
- **search_datasets**: Returns matching dataset codes and names. Use this to find the right dataset code before querying data.

Search Eurostat dataset catalog by keyword
- **get_dataset_metadata**: Shows all available dimensions, code lists, and possible filter values. Use this before querying to understand what filters are available.

Get metadata for a Eurostat dataset: dimensions, codes, frequencies
- **get_dataset**: Provide the dataset code and optional dimension filters. Find codes via search_datasets or the Eurostat Data Browser.

Query any Eurostat dataset by code with flexible filters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Eurostat Discovery — Dataset Catalog Explorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find datasets related to housing prices"

**🤖 AI Agent:**
> 🔍 **Search: 'housing prices'**

Found 12 matching datasets:
1. prc_hpi_q — House Price Index (quarterly)
2. prc_hpi_a — House Price Index (annual)
3. ilc_lvho02 — Housing cost overburden rate
4. enpr_lphp — Labour cost in housing construction
...

Use get_dataset with code 'prc_hpi_q' to retrieve data.

---

**👤 You:**
> "What dimensions are available in the GDP dataset?"

**🤖 AI Agent:**
> 📋 **Metadata: namq_10_gdp**

Dimensions:
- geo: 42 countries (EU27 + EEA + candidates)
- time: 1995-Q1 to 2024-Q3
- unit: 8 options (CP_MEUR, CLV10_MEUR, PC_GDP...)
- na_item: 15 components (B1GQ=GDP, P3, P5G...)
- s_adj: SCA, NSA, CA
- freq: Q (quarterly)

Use these dimension codes as filter parameters.

---

**👤 You:**
> "Get the house price index for Germany and France since 2020"

**🤖 AI Agent:**
> 🏠 **House Price Index (2015=100)**

| Quarter | 🇩🇪 Germany | 🇫🇷 France |
|---------|------------|----------|
| 2020-Q1 | 128.3 | 112.1 |
| 2022-Q4 | 152.1 | 129.4 |
| 2024-Q2 | 138.7 | 122.8 |

German prices peaked in 2022 then corrected -8.8%. France more stable.


## ❓ FAQ

**Q: How many datasets does Eurostat have?**
Over **7,000 datasets** covering 9 statistical themes. Use the search_datasets tool to find any dataset by keyword, then get_dataset_metadata to understand its dimensions before querying.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eurostat-discovery-dataset-catalog-explorer](https://vinkius.com/mcp/eurostat-discovery-dataset-catalog-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Eurostat Discovery — Dataset Catalog Explorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `eurostat-discovery-dataset-catalog-explorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Eurostat Discovery — Dataset Catalog Explorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eurostat-discovery-dataset-catalog-explorer": {
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
