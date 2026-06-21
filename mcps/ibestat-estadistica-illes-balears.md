# IBESTAT (Estadística Illes Balears) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ibestat-estadistica-illes-balears)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access official statistical data from the Balearic Islands — query operations, resources, and detailed datasets directly from your AI agent.

## Description
Connect to the **IBESTAT (Institut d'Estadística de les Illes Balears)** and bring official public data into your AI workflows. This server provides direct access to the comprehensive statistical catalog of the Balearic Islands.

### What you can do

- **Browse Operations** — List all available statistical operations and studies conducted by the institute.
- **Discover Resources** — Identify specific tables and datasets associated with any statistical operation using its unique ID.
- **Fetch Raw Data** — Retrieve actual statistical figures in JSON, CSV, or XML formats for deep analysis.
- **Metadata Access** — Get the underlying context, definitions, and structural information for specific operations to ensure data accuracy.

### How it works

1. Subscribe to this server
2. Provide a User Agent identifier for API requests
3. Start querying Balearic statistics from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly pull official regional data for reports and visualizations without manual downloads.
- **Researchers** — access historical and current socio-economic indicators of the Balearic Islands via natural language.
- **Developers** — integrate real-time public statistics into applications and dashboards using the structured API output.


## Available Tools
- **get_data**: Retrieve statistical data for a specific resource
- **get_metadata**: Retrieve metadata for a specific operation
- **list_operations**: List all statistical operations available in IBESTAT
- **list_resources**: g., specific tables) for a given statistical operation ID.

Retrieve resources associated with a specific operation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IBESTAT (Estadística Illes Balears)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available statistical operations from IBESTAT."

**🤖 AI Agent:**
> I have retrieved the list of statistical operations. There are several categories available, including 'Population' (ID: 01), 'Tourism' (ID: 05), and 'Economy' (ID: 10). Which area would you like to explore further?

---

**👤 You:**
> "Show me the resources available for the statistical operation with ID '0201'."

**🤖 AI Agent:**
> For operation '0201', I found the following resources: 'Table 1: Annual Growth', 'Table 2: Regional Distribution', and 'Table 3: Historical Series'. Would you like to fetch the data for one of these?

---

**👤 You:**
> "Get the data for operation '0201' and resource 'T1' in English and JSON format."

**🤖 AI Agent:**
> I've fetched the data for resource 'T1'. It contains the annual growth metrics for the requested period. [JSON Data Displayed]. Would you like me to analyze these numbers for you?


## ❓ FAQ

**Q: How can I find out which statistical tables are available for a specific study?**
Use the `list_resources` tool with the specific `operationId`. It will return a list of all available resources (tables) associated with that statistical operation.

**Q: Can I retrieve the statistical data in different languages?**
Yes. When using the `get_data` tool, you can specify the `lang` parameter. Supported languages typically include Catalan ('ca'), Spanish ('es'), and English ('en').

**Q: What formats are available for downloading data?**
The `get_data` tool allows you to choose between 'json', 'xml', and 'csv' formats via the `format` parameter, making it easy to integrate with different analysis tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ibestat-estadistica-illes-balears](https://vinkius.com/mcp/ibestat-estadistica-illes-balears)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IBESTAT (Estadística Illes Balears)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ibestat-estadistica-illes-balears` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IBESTAT (Estadística Illes Balears)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ibestat-estadistica-illes-balears": {
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
