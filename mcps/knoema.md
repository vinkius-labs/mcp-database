# Knoema MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/knoema)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access global statistics — search datasets, retrieve time-series data, and audit economic indicators.

## Description
Connect your AI agent to **Knoema**, the most comprehensive source of global decision-making data.

### What you can do

- **Dataset Discovery** — Search through millions of datasets from official sources like IMF, World Bank, and UN
- **Data Retrieval** — Fetch precise time-series data using mnemonics for your analysis and forecasting
- **Metadata Auditing** — Get detailed information about data sources, units, and frequencies
- **Granular Search** — Find specific indicators (e.g., GDP, CPI, Crude Oil Price) across multiple providers
- **Visualization Support** — Access atlas and dashboard resources for visual data context

### How it works

1. Subscribe to this server
2. Enter your Knoema Client ID and Secret (from the Developer Portal)
3. Start querying global statistics directly from your chat client

### Use Cases

- **Economic Analysis** — gather historical and current macro indicators for market research
- **Business Planning** — use demographic and sector data to inform strategy
- **Scientific Research** — find environmental and social datasets for academic or professional studies


## Available Tools
- **search_datasets**: Returns dataset IDs and metadata. Use this to find the correct data source for your statistics.

Search for datasets in Knoema
- **get_dataset_metadata**: Critical for understanding what variables are available.

Get metadata for a specific dataset
- **list_data_topics**: g., Agriculture, Economy, Demographics).

List all available data topics in Knoema
- **get_data_series**: Requires dataset ID and a list of mnemonics.

Get specific data series
- **list_dataset_regions**: ) supported by a specific dataset.

List regions available in a dataset
- **list_data_units**: g., Percentage, USD, Kilograms).

List measurement units
- **get_latest_dataset_data**: Get the most recent data points for a dataset
- **search_data_series**: More granular than dataset search. Ideal for finding specific indicators.

Search for specific data series across all datasets
- **list_data_frequencies**: g., Annual, Quarterly, Monthly).

List available data frequencies
- **get_knoema_resource**: Get a generic frontend resource


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Knoema** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for datasets about renewable energy in Europe"

**🤖 AI Agent:**
> I've found 12 datasets related to renewable energy in Europe, including 'Eurostat: Energy statistics' and 'IRENA: Renewable Capacity'. Which one should we analyze?

---

**👤 You:**
> "Get the metadata for dataset 'IMFWEOS2024Oct'"

**🤖 AI Agent:**
> Retrieved metadata for 'IMF World Economic Outlook (October 2024)'. It contains 45 indicators for 196 countries, covering 1980-2029. Indicators include GDP, Inflation, and Unemployment.

---

**👤 You:**
> "Search for crude oil price series"

**🤖 AI Agent:**
> I found multiple series for crude oil prices. The most relevant are 'Crude Oil (Brent)' from World Bank and 'WTI Crude' from EIA. Would you like to fetch the latest data for these?


## ❓ FAQ

**Q: Where do I get my Knoema API credentials?**
Visit the **Knoema Developer Portal** (knoema.com/dev), create an application, and you will receive a Client ID and Client Secret.

**Q: How can I find a specific dataset ID?**
Use the `search_datasets` tool with relevant keywords. The tool will return a list of matching datasets along with their unique IDs.

**Q: What is a mnemonic in Knoema?**
A mnemonic is a short, human-readable code used to identify a specific data series within a dataset (e.g., 'NGDP' for Nominal GDP).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/knoema](https://vinkius.com/mcp/knoema)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Knoema** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `knoema` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Knoema** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "knoema": {
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
