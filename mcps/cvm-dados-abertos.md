# CVM Dados Abertos MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cvm-dados-abertos)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cvm-dados-abertos-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cvm-dados-abertos-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access Brazilian capital markets data directly from the CVM Open Data portal — query investment funds, listed companies, and financial reports.

## Description
Connect your AI agent to the **CVM (Comissão de Valores Mobiliários)** Open Data portal and explore the Brazilian financial market through natural conversation.

### What you can do

- **Dataset Exploration** — List all available datasets or search for specific topics like 'investment funds' or 'listed companies'.
- **Deep Metadata Inspection** — Fetch complete metadata for specific datasets, including update frequency, tags, and organizational ownership.
- **Resource Access** — Retrieve direct links and metadata for specific data resources (CSV, XML, or PDF files) within the portal.
- **Organizational Mapping** — List the CVM departments and thematic groups responsible for publishing specific sets of financial data.
- **Market Research** — Quickly find registration data (fi-cad) or daily reports (infodiario) without navigating complex web directories.

### How it works

1. Subscribe to this server
2. Enter your CVM API Key (optional for public access, but recommended for higher limits)
3. Start querying Brazilian financial data from Claude, Cursor, or any MCP client

### Who is this for?

- **Financial Analysts** — instantly find the latest registration data for investment funds or corporate filings.
- **Data Scientists** — automate the discovery of CSV resources for financial modeling and market analysis.
- **Compliance Officers** — verify organizational data and thematic groupings for regulatory reporting.


## Available Tools
- **list_groups**: g., "Fundos de Investimento", "Companhias").

List thematic groups
- **list_organizations**: g., CVM departments) that publish data on the portal.

List organizations that publish data
- **list_datasets**: List all datasets available on the CVM portal
- **search_datasets**: Search for datasets matching specific criteria
- **get_dataset**: Get complete metadata for a specific dataset
- **get_resource**: Get metadata for a specific resource


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CVM Dados Abertos** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all datasets available on the CVM portal."

**🤖 AI Agent:**
> I have retrieved the list of available datasets. There are over 50 packages including 'Companhias Abertas', 'Fundos de Investimento', and 'Ofertas Públicas'. Which category interests you?

---

**👤 You:**
> "Search for datasets related to 'fundos'."

**🤖 AI Agent:**
> Searching for 'fundos'... I found several matches: 'fi-cad' (Registration), 'fi-doc-eventual' (Occasional docs), and 'fi-doc-infodiario' (Daily info). Would you like to see the details for 'fi-cad'?

---

**👤 You:**
> "Get the metadata for the dataset 'fi-cad'."

**🤖 AI Agent:**
> I've retrieved the metadata for 'fi-cad'. It contains registration information for investment funds and includes 12 resources (CSV files). Would you like the download link for the most recent file?


## Installation & Usage

To install and use the **CVM Dados Abertos** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cvm-dados-abertos](https://vinkius.com/mcp/cvm-dados-abertos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
