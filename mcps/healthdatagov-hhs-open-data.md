# HealthData.gov (HHS Open Data) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/healthdatagov-hhs-open-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/healthdatagov-hhs-open-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/healthdatagov-hhs-open-data-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **HealthData.gov (HHS Open Data)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/healthdatagov-hhs-open-data](https://vinkius.com/mcp/healthdatagov-hhs-open-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
