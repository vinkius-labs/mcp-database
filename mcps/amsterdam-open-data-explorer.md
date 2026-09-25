# Amsterdam Open Data Explorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/amsterdam-open-data-explorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Keyless explorer over all 122+ datasets of Amsterdam's DSO open-data platform: list datasets, inspect their resources, browse any table and query the data catalog — no API key.

## Description
The meta-interface to Amsterdam's open data. Instead of one dataset, this MCP lets an agent discover and query the whole DSO Dataplatform: the live dataset index, per-dataset API specs, generic table access and the city's data catalog of products and data teams.

### What you can do
- **List datasets** — all 122+ services with name, description, tags and API URL; filter by keyword or tag
- **Inspect a dataset** — the OpenAPI spec for any dataset: which resources it exposes and which operations (GET/POST) each supports
- **Browse any dataset** — generic fetcher for any dataset + resource: optional filters, sort, page, page size and field projection
- **Data catalog** — the city's catalogued data products and the 26 data teams that own them

### Who is this for
Agents that need to explore Amsterdam open data without knowing the dataset names up front, prototyping against new datasets, and building on top of anything the DSO platform exposes.


## Available Tools (5)
- **list_datasets**: Use it to discover which datasets exist before browsing one. Optionally filter by keyword or tag.

List all open datasets published by the city of Amsterdam
- **get_dataset_info**: Returns the dataset metadata plus the list of resources (API paths and their operations), so you know which resource names to pass to browse_dataset.

Get full metadata and the OpenAPI resources of one dataset
- **list_data_products**: Optionally filter by keyword or paginate.

List the city data products catalog
- **browse_dataset**: Discover the dataset folder, version and resource names with list_datasets / get_dataset_info first. Accepts comma-separated field=value filters plus the standard pagination, sorting and field-projection parameters.

Browse any resource of any city dataset (generic fetcher)
- **list_data_teams**: Optionally filter by keyword.

List the city data teams that own the data products


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amsterdam Open Data Explorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which Amsterdam datasets are about water?"

**🤖 AI Agent:**
> list_datasets with a 'water' keyword returns the matching dataset rows: service name, short description, tags, open-data URL and API URL. Inspect one with get_dataset_info.

---

**👤 You:**
> "What resources does the bomen dataset expose?"

**🤖 AI Agent:**
> get_dataset_info for 'bomen' fetches its OpenAPI spec and lists the resources with their supported operations: stamgegevens, kapenherplant, stormmeldingen, veiligheidsinspecties and more — use these names with browse_dataset.

---

**👤 You:**
> "Fetch the first 10 rows of bag nummeraanduidingen."

**🤖 AI Agent:**
> browse_dataset with dataset 'bag' and resource 'nummeraanduidingen' (page size 10) returns the address rows with pagination fields, so you can page deeper into the full register.


## ❓ FAQ

**Q: Do I need an API key?**
No. The DSO dataset index, the per-dataset OpenAPI specs and the generic table access are public (OPENBAAR). Some individual datasets are marked as requiring a key in their index entry — the dataset info response shows the authentication requirement, so check it before assuming access.

**Q: How do I find the right resource names?**
Call get_dataset_info for the dataset: it fetches the live OpenAPI spec and lists the exposed resources and their operations. Use the resource name (usually the Dutch word) with browse_dataset — e.g. 'stamgegevens' for bomen, 'nummeraanduidingen' for bag.

**Q: What does browse_dataset return?**
A page of the dataset's rows: the items array, current page number and page size, plus a next-link (next) when more pages exist. Filters are passed as comma-separated field=value pairs and only applied when the dataset actually supports that filter field.

**Q: What is the difference between the catalog and the datasets?**
The dataset index (list_datasets) covers the machine-readable REST APIs. The data catalog (list_data_products / list_data_teams) covers the city's curated catalogue of data products and the 26 data teams that produce and own them — useful for mapping a question to the right dataset or owner.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/amsterdam-open-data-explorer](https://vinkius.com/en/ai-agent-connect/amsterdam-open-data-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amsterdam Open Data Explorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `amsterdam-open-data-explorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amsterdam Open Data Explorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amsterdam-open-data-explorer": {
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
