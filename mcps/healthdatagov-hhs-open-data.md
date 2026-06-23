# HealthData.gov (HHS Open Data) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/healthdatagov-hhs-open-data)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access and query thousands of U.S. health datasets from HHS — browse the catalog and perform deep data analysis via SoQL.

## Description
Connect your AI agent to **HealthData.gov**, the central clearinghouse for open data from the U.S. Department of Health & Human Services (HHS). This MCP server empowers your agent to discover and analyze vast amounts of public health, social service, and Medicare/Medicaid data.

### What you can do

- **Catalog Discovery** — Search and list thousands of available datasets, views, and resources across the entire HHS ecosystem.
- **Deep Data Querying** — Use Socrata Query Language (SoQL) to filter, sort, and aggregate data from specific datasets (e.g., hospital capacity, COVID-19 statistics, or provider directories).
- **Precision Filtering** — Apply complex `$where`, `$select`, and `$order` parameters to extract exactly the records you need without downloading massive files.
- **Real-time Research** — Fetch the latest updates on public health metrics directly into your conversation for immediate analysis.

### How it works

1. Subscribe to this server
2. (Optional) Enter your HealthData.gov/Socrata App Token for higher rate limits
3. Start querying public health data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists & Researchers** — quickly prototype data queries and fetch subsets of health data for analysis.
- **Public Health Officials** — monitor live datasets and trends across different states and regions.
- **Developers** — integrate official HHS data into applications by testing queries through a natural language interface.


## Available Tools (2)
- **get_catalog**: Get catalog of datasets from HealthData.gov
- **query_dataset**: g., 6xf2-c3ie) and SoQL parameters.

Query a specific dataset on HealthData.gov using SoQL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HealthData.gov (HHS Open Data)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search the HealthData.gov catalog for datasets related to 'COVID-19 hospitalizations'."

**🤖 AI Agent:**
> I found several datasets. The most relevant is 'COVID-19 Reported Patient Impact and Hospital Capacity by State' (ID: 6xf2-c3ie). Would you like me to query the latest records from this dataset?

---

**👤 You:**
> "Query dataset '6xf2-c3ie' to show the top 5 states with the highest adult ICU utilization."

**🤖 AI Agent:**
> I've queried the dataset sorting by ICU utilization. The top 5 states currently reporting the highest percentages are: 1. Alabama, 2. Georgia, 3. Texas, 4. Florida, 5. Mississippi. Would you like the specific percentage values?

---

**👤 You:**
> "List the first 10 datasets available in the health catalog."

**🤖 AI Agent:**
> Fetching the first 10 entries from the HealthData.gov catalog... I've retrieved datasets including 'Medicare Provider Utilization', 'Community Health Status Indicators', and 'National Health Nutrition Examination Survey'. Which one would you like to explore?


## ❓ FAQ

**Q: How do I find a specific dataset about 'Medicare'?**
Use the `get_catalog` tool and provide 'Medicare' in the `q` parameter. This will return a list of relevant datasets along with their unique identifiers (dataset_id).

**Q: Can I filter results to only show data from a specific state?**
Yes! When using `query_dataset`, use the `$where` parameter with a SoQL filter like `state='NY'`. You can also use `$select` to pick specific columns.

**Q: Is an API key required to access this data?**
No, the data is public. However, providing a `HEALTHDATA_APP_TOKEN` is recommended for higher rate limits if you plan to perform many queries.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/healthdatagov-hhs-open-data](https://vinkius.com/mcp/healthdatagov-hhs-open-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HealthData.gov (HHS Open Data)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `healthdatagov-hhs-open-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HealthData.gov (HHS Open Data)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "healthdatagov-hhs-open-data": {
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
