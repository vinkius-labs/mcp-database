# data.world MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dataworld)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Equip your AI agent to discover and manage data assets, projects, and queries directly via the data.world API.

## Description
Integrate **data.world**, the enterprise data catalog and collaborative data platform, directly into your AI workflow. Discover datasets, monitor data projects, and explore saved queries and insights using natural language.

### What you can do

- **Data Discovery** — Search the entire data.world catalog for relevant datasets and projects.
- **Asset Management** — List and retrieve detailed information for datasets and projects you own or manage.
- **Collection Oversight** — Explore curated collections of data assets within your organization.
- **Query & Insight Access** — List saved SQL/SPARQL queries and published insights for your data projects.

### How it works

1. Connect the data.world integration to your AI assistant.
2. Authorize using your data.world API Token (found in your user settings).
3. Manage your data catalog and collaborative projects through intuitive conversation.

### Who is this for?

- **Data Scientists & Analysts** — Quickly find datasets and retrieve query definitions for research.
- **Data Stewards** — Monitor project status and audit data assets via chat.
- **Knowledge Managers** — Explore organizational collections and insights during data planning.


## Available Tools (10)
- **get_dataset_details**: Includes field definitions, file listings, tags, and license information.

Get detailed information for a specific dataset
- **get_my_profile**: world. Returns profile attributes including username, display name, and account-level permissions.

Retrieve metadata for the current authenticated user
- **get_project_details**: Resolves project members, associated objective, and the current status of linked resources.

Get detailed information for a specific project
- **list_recent_activity**: Returns a stream of activity logs including dataset updates, project contributions, and new collection entries.

List recent activities in your data.world account
- **list_my_collections**: Returns collection identifiers, descriptions, and item counts.

List all collections you own or manage
- **list_dataset_queries**: Returns a list of saved query definitions, including their language (SQL/SPARQL) and creator metadata.

List all saved SQL or SPARQL queries for a dataset
- **list_my_datasets**: world catalog for datasets owned by the authenticated user. Returns a list of dataset metadata including title, visibility (public/private), and timestamp of last modification.

List all datasets you own on data.world
- **list_project_insights**: Insights represent documented findings and data visualizations attached to the project workspace.

List all insights published within a project
- **list_my_projects**: Returns project summaries including role (owner/contributor), creation date, and linked datasets.

List all projects you own on data.world
- **search_catalog**: world index. Supports full-text search across titles, descriptions, and tags. Returns a ranked list of matching resources.

Search for datasets and projects across data.world


## 💬 Prompt Examples

Here are some examples of how you can interact with the **data.world** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for datasets related to 'Global Climate Change'."

**🤖 AI Agent:**
> I've found several datasets related to 'Global Climate Change', including 'NASA GISS Surface Temperature' and 'UN Statistics on Emissions'. Would you like to see the details for any of these?

---

**👤 You:**
> "List all SQL queries saved in my project 'Sales Analysis 2024'."

**🤖 AI Agent:**
> Project 'Sales Analysis 2024' has 3 saved SQL queries: 'Monthly Revenue Recap', 'Top Performing Regions', and 'Churn Rate Analysis'. Should I retrieve the SQL definition for any of them?

---

**👤 You:**
> "Show me the insights published in dataset 'Retail Trends'."

**🤖 AI Agent:**
> I've found 2 insights for 'Retail Trends': 'Q1 Growth Patterns' and 'Customer Demographics Shift'. Both were published by 'DataTeam_Alpha'. Would you like to see the full content of these insights?


## ❓ FAQ

**Q: How do I get a data.world API Token?**
Log in to data.world, go to your user settings, and navigate to the **Advanced > API Tokens** section to generate a new token.

**Q: Can the agent run SQL queries?**
This integration currently focuses on discovering assets and retrieving saved query definitions. Executing arbitrary SQL queries is managed via the data.world interface or specialized SDKs.

**Q: Does the integration support private datasets?**
Yes, as long as the provided API Token has the necessary permissions, the agent can list and retrieve information for any dataset you have access to, including private ones.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dataworld](https://vinkius.com/mcp/dataworld)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **data.world** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dataworld` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **data.world** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dataworld": {
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
