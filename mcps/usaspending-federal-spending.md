# USAspending (Federal Spending) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/usaspending-federal-spending)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/usaspending-federal-spending-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/usaspending-federal-spending-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Analyze US federal spending data — query agency budgets, track awards, and explore geographic spending patterns directly from your AI agent.

## Description
Connect to the official **USAspending** database and gain unprecedented transparency into how the United States government allocates its budget. This server allows any AI agent to query real-time federal financial data, from high-level agency overviews to specific contract details.

### What you can do

- **Agency Insights** — Retrieve comprehensive overviews of toptier agencies, including their budgetary resources and obligations.
- **Award Tracking** — Search and filter through millions of federal awards, contracts, and grants using advanced criteria.
- **Geographic Analysis** — Break down spending by state, county, or congressional district to see where the money is going.
- **Sub-Agency Breakdown** — List specific offices and sub-agencies within a department to identify internal spending distribution.
- **Historical Trends** — Analyze spending and new award counts over time to identify fiscal patterns.

### How it works

1. Subscribe to this server
2. Enter your USAspending API Key (if required for higher rate limits)
3. Start auditing federal spending from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Policy Researchers** — quickly gather data on agency obligations and budgetary resources for reports
- **Journalists** — track federal contracts and grants in specific regions or categories for investigative stories
- **Data Analysts** — export and analyze spending trends over time across different government sectors


## Available Tools
- **autocomplete_awarding_agency**: Awarding agencies matching search text
- **autocomplete_glossary**: Glossary terms matching search text
- **autocomplete_location**: Locations based on search text
- **autocomplete_recipient**: Recipient names and UEI based on search text
- **bulk_download_awards**: Generates ZIP file of award data in CSV
- **download_search**: ZIP file for Awards, Subawards, and Transactions
- **get_agency_awards_count**: Count of award types for agencies in a fiscal year
- **get_agency_awards**: Get summary of transactions and obligations for an agency
- **get_agency_budgetary_resources**: Get budgetary resources and obligations by fiscal year
- **get_agency_overview**: Get agency overview for details page
- **get_agency_sub_agencies**: List sub-agencies and offices with obligated amounts
- **get_award_funding**: Federal account and agency funding info for an award
- **get_award**: Get details about a specific award
- **get_award_types**: Map of award types by grouping
- **get_data_dictionary**: JSON structure of the Rosetta Crosswalk Data Dictionary
- **get_disaster_agency_spending**: Insights on agencies receiving disaster funding
- **get_disaster_award_amount**: Obligation and outlay aggregations for disaster awards
- **get_disaster_overview**: Overview of disaster/emergency funding and spending
- **get_download_status**: Current status of a requested download job
- **get_glossary**: List of glossary terms and definitions
- **get_recipient_children**: Recipient details based on identifier
- **get_recipient_state**: Basic information about a specified state
- **get_recipient**: Individual recipient details
- **get_subawards**: Subawards related to a specific parent award
- **get_toptier_agencies**: All toptier agencies and relevant data
- **get_transactions**: Transactions related to a specific parent award
- **list_recipients**: List of recipients in the database
- **search_new_awards_over_time**: List of time periods with new awards
- **search_spending_by_award**: Search and filter awards
- **search_spending_by_category**: g., agency, recipient, CFDA).

Grouped spending data for visualizations
- **search_spending_by_geography**: Spending by state, county, or congressional district
- **search_spending_over_time**: Aggregated transaction amounts over time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **USAspending (Federal Spending)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the agency overview for the Department of Energy using toptier code 089."

**🤖 AI Agent:**
> I've retrieved the overview for the Department of Energy (089). For the current fiscal year, they have total budgetary resources of $X billion and have obligated $Y billion across various programs.

---

**👤 You:**
> "List all sub-agencies and their obligated amounts for the Department of Justice (toptier code 015)."

**🤖 AI Agent:**
> The Department of Justice (015) has several sub-agencies. The Federal Bureau of Investigation (FBI) has obligated $A, while the Drug Enforcement Administration (DEA) has obligated $B. Would you like a full breakdown?

---

**👤 You:**
> "Search for spending by geography for the state of Texas in fiscal year 2023."

**🤖 AI Agent:**
> In fiscal year 2023, federal spending in Texas was distributed across various counties. Harris County received the highest amount at $C, followed by Dallas County at $D. Most of this was categorized under 'Contracts'.


## Installation & Usage

To install and use the **USAspending (Federal Spending)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/usaspending-federal-spending](https://vinkius.com/mcp/usaspending-federal-spending)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
