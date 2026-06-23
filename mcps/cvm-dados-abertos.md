# CVM Dados Abertos MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cvm-dados-abertos)
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


## Available Tools (6)
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


## ❓ FAQ

**Q: How can I find the most recent data for a specific investment fund?**
Use the `search_datasets` tool with keywords like 'fundos' or 'fi-cad'. Once you identify the dataset, use `get_dataset` to list all available resources, which typically include the most recent CSV files.

**Q: Can I get the direct download link for a data file?**
Yes! Use the `get_resource` tool with a specific Resource ID. The response will include the `url` field, which is the direct link to the raw data (e.g., a CSV file).

**Q: What are thematic groups in the CVM portal?**
Thematic groups categorize datasets by market segment. Use `list_groups` to see categories like 'Fundos de Investimento', 'Companhias', and 'Auditores Independentes' to better navigate the available data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cvm-dados-abertos](https://vinkius.com/mcp/cvm-dados-abertos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CVM Dados Abertos** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cvm-dados-abertos` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CVM Dados Abertos** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cvm-dados-abertos": {
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
