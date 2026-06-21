# BEA (Bureau of Economic Analysis) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bea-bureau-of-economic-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access official US economic statistics including GDP, personal income, and industry data directly from the Bureau of Economic Analysis.

## Description
The **BEA (Bureau of Economic Analysis)** MCP server provides a direct bridge to one of the world's most comprehensive sources of economic data. Empower your AI agent to retrieve, analyze, and report on the health of the US economy with precision.

### What you can do

- **Dataset Discovery** — Browse all available economic datasets including NIPA (National Income and Product Accounts), Regional, and Industry data.
- **Parameter Exploration** — Identify the specific filters and variables required for any dataset to ensure accurate queries.
- **Valid Value Lookup** — Retrieve lists of valid codes for parameters like TableID or Frequency to avoid API errors.
- **Data Retrieval** — Fetch raw economic figures, growth rates, and historical statistics directly into your conversation or analysis tool.

### How it works

1. Subscribe to this server
2. Enter your BEA API Key
3. Start querying economic indicators from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Economists & Researchers** — Quickly pull historical GDP or income data without manual CSV downloads.
- **Financial Analysts** — Integrate macroeconomic trends into market analysis and forecasting models.
- **Data Scientists** — Automate the ingestion of government-verified economic signals for machine learning projects.


## Available Tools
- **get_dataset_list**: g., NIPA, Regional, GDPByIndustry).

List available BEA datasets
- **get_data**: Pass dataset-specific parameters as a JSON string.

Retrieve economic data from a BEA dataset
- **get_parameter_list**: List parameters for a specific BEA dataset
- **get_parameter_values**: List valid values for a BEA dataset parameter


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BEA (Bureau of Economic Analysis)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all the available datasets from the Bureau of Economic Analysis."

**🤖 AI Agent:**
> I've retrieved the list of available BEA datasets. You can access data from NIPA (National Income and Product Accounts), NIUnderlyingDetail, FixedAssets, ITA (International Transactions), and several others. Which one would you like to explore?

---

**👤 You:**
> "What parameters do I need to query the NIPA dataset?"

**🤖 AI Agent:**
> For the NIPA dataset, you typically need the following parameters: 'TableName' or 'TableID', 'Frequency' (e.g., A for Annual, Q for Quarterly), and 'Year'. I can help you find valid values for these using the parameter values tool.

---

**👤 You:**
> "Get the GDP data for 2023 from the NIPA dataset using Table T10101."

**🤖 AI Agent:**
> I am fetching the data for NIPA Table T10101 for the year 2023... The data shows Real Gross Domestic Product increased at an annual rate of 2.5 percent in 2023. Would you like a breakdown by quarter?


## ❓ FAQ

**Q: How can I see which economic datasets are available?**
You can use the `get_dataset_list` tool. It will return a comprehensive list of all datasets currently supported by the BEA API, such as NIPA, NIUnderlyingDetail, and FixedAssets.

**Q: How do I know what filters or parameters to use for a specific dataset?**
First, use `get_parameter_list` with the dataset name to see required fields. Then, use `get_parameter_values` to find valid inputs (like specific Year or TableID) for those parameters.

**Q: Can I fetch actual GDP or income figures directly?**
Yes. Use the `get_data` tool. You will need to provide the dataset name and a JSON string of parameters (e.g., TableName, Frequency, Year) to retrieve the specific economic observations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bea-bureau-of-economic-analysis](https://vinkius.com/mcp/bea-bureau-of-economic-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BEA (Bureau of Economic Analysis)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bea-bureau-of-economic-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BEA (Bureau of Economic Analysis)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bea-bureau-of-economic-analysis": {
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
