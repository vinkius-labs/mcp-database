# ERS USDA (Economic Research) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ers-usda-economic-research)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access USDA Economic Research Service data, specifically the Agricultural Resource Management Survey (ARMS), covering farm finances and production.

## Description
Connect to the **USDA Economic Research Service (ERS)** and query the Agricultural Resource Management Survey (ARMS) directly. This server provides comprehensive access to the primary source of information on the financial condition, production practices, and resource use of America's farm businesses.

### What you can do

- **Survey Data Retrieval** — Fetch detailed financial and production data from U.S. farms using specific years, reports, or variables.
- **Geographic Analysis** — List all available ARMS States and retrieve metadata specific to regional agricultural economies.
- **Historical Trends** — Access all available survey years to perform longitudinal analysis of farm income and expenses.
- **Variable Metadata** — Inspect detailed definitions and metadata for variables used in the ARMS dataset to ensure accurate data interpretation.
- **Farm Classification** — Query specific farm types and categories (like farm typology or operator households) to segment your research.

### How it works

1. Subscribe to this server
2. Enter your ERS USDA API Key
3. Start querying agricultural economic data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Agricultural Economists** — quickly pull survey results for income statements and balance sheets without manual exports.
- **Data Analysts** — integrate official government agricultural metrics into broader economic models or reports.
- **Policy Researchers** — analyze farm household characteristics and production practices across different U.S. states.


## Available Tools (7)
- **get_arms_farmtypes**: Get all ARMS Farm Types
- **get_arms_reports**: Get available ARMS reports and variables
- **get_arms_states**: Get all ARMS States and available metadata
- **get_arms_surveydata**: S. farms. Requires year AND at least one of report or variable.

Retrieve ARMS survey results
- **get_arms_variables**: Get detailed metadata for ARMS variables
- **get_arms_years**: Get all available ARMS years
- **get_arms_categories**: List ARMS categories and subcategories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ERS USDA (Economic Research)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all available years for the ARMS survey data."

**🤖 AI Agent:**
> I've retrieved the available years for the ARMS dataset. Data is available for a wide range of years, including recent periods like 2021 and 2022. Which year would you like to analyze?

---

**👤 You:**
> "Get the income statement survey data for the year 2022."

**🤖 AI Agent:**
> Fetching the 2022 income statement data... I have retrieved the financial results. This includes metrics for gross cash farm income, total cash expenses, and net cash farm income across the surveyed regions.

---

**👤 You:**
> "List the different farm types available in the ERS ARMS dataset."

**🤖 AI Agent:**
> I've found the available farm types. Categories include 'operator households', 'commercial farms', and various other classifications based on production and economic size.


## ❓ FAQ

**Q: What is required to fetch specific survey results using this server?**
To use the `get_arms_surveydata` tool, you must provide at least one year and either a 'report' name (like income+statement) or a specific 'variable' ID (like igcfi).

**Q: Can I see which states are available in the ARMS dataset?**
Yes! Use the `get_arms_states` tool to retrieve a list of all U.S. states covered by the survey along with their associated metadata.

**Q: How do I find the meaning of a specific variable code like 'igcfi'?**
You can use the `get_arms_variables` tool to fetch detailed metadata and descriptions for all variables used in the Agricultural Resource Management Survey.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ers-usda-economic-research](https://vinkius.com/mcp/ers-usda-economic-research)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ERS USDA (Economic Research)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ers-usda-economic-research` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ERS USDA (Economic Research)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ers-usda-economic-research": {
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
