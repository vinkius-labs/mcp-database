# OpenDataSUS MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opendatasus)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/opendatasus-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/opendatasus-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access Brazilian public health data (SUS) directly from your AI. Query datasets, search resources, and analyze health statistics from the official portal.

## Description
Connect to the **OpenDataSUS** portal to explore and analyze Brazilian public health information through natural language. This server interfaces with the CKAN-based API of the Ministry of Health.

### What you can do

- **Dataset Discovery** — List all available datasets, search for specific health topics (like COVID-19 or vaccination), and browse by tags or categories.
- **Metadata Inspection** — Retrieve detailed metadata for packages and individual resources to understand data provenance and structure.
- **Deep Data Querying** — Use the DataStore search to filter and retrieve actual rows from CSV and Excel resources directly into your conversation.
- **Organizational Browsing** — List data providers and organizations to find specific departmental records.

### How it works

1. Subscribe to this server
2. (Optional) Enter your OpenDataSUS API Key for higher rate limits
3. Start querying Brazilian health data from Claude, Cursor, or any MCP client

### Who is this for?

- **Data Scientists & Researchers** — quickly find and sample epidemiological data without manual downloads
- **Public Health Analysts** — monitor health indicators and dataset updates through simple queries
- **Developers** — integrate official Brazilian health data into applications and dashboards with ease


## Available Tools
- **datastore_search**: Search and filter data within a resource
- **group_list**: List all groups (categories)
- **organization_list**: List all organizations (data providers)
- **package_list**: List all dataset names in the OpenDataSUS portal
- **package_search**: Search for datasets matching specific criteria
- **package_show**: Get full metadata of a specific dataset
- **resource_show**: Get metadata for a specific resource
- **tag_list**: List all tags used across datasets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenDataSUS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for datasets related to 'vacinacao covid' in OpenDataSUS."

**🤖 AI Agent:**
> I found several datasets. The most relevant is 'Campanha Nacional de Vacinação contra Covid-19'. Would you like to see the available resources (CSV/Excel) for this package?

---

**👤 You:**
> "List all health organizations providing data on the portal."

**🤖 AI Agent:**
> I've retrieved the list of organizations. It includes 'Ministério da Saúde', 'Secretaria de Vigilância em Saúde', and others. Which one would you like to explore?

---

**👤 You:**
> "Query the first 5 rows of the resource with ID 'd3848184-5077-4667-835d-591d67641bb9'."

**🤖 AI Agent:**
> Accessing the DataStore... Here are the first 5 records from that resource, showing columns like 'municipio', 'data_notificacao', and 'casos_confirmados'.


## Installation & Usage

To install and use the **OpenDataSUS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opendatasus](https://vinkius.com/mcp/opendatasus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
