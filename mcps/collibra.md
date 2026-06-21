# Collibra MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/collibra)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Enable your AI agent to manage data assets, domains, and communities via the Collibra Data Intelligence API.

## Description
Connect your AI to **Collibra**, the data intelligence platform that helps organizations find, understand, and trust their data.

### What you can do

- **Asset Search** — Search for data assets by name, type, or domain and retrieve their full metadata.
- **Community Browsing** — List all communities and domains to navigate your data governance structure.
- **Asset Details** — Inspect any asset's attributes, responsibilities, and relationships.

### How it works

1. Add the Collibra integration to your AI toolset.
2. Provide your instance URL, username, and password.
3. Browse your data catalog via natural language.

### Who is this for?

- **Data Stewards** — Find and inspect assets without navigating the full Collibra UI.
- **Data Engineers** — Look up table/column definitions and ownership from chat.
- **Compliance Teams** — Verify data classifications and governance policies quickly.


## Available Tools
- **create_asset**: Create a new asset in Collibra
- **get_asset**: Retrieve detailed information about a specific asset
- **get_community_details**: Retrieve detailed information about a specific community
- **list_asset_types**: Retrieve a list of available asset types
- **list_assets**: Retrieve a list of assets in Collibra
- **list_communities**: Retrieve a list of communities in Collibra
- **list_domain_types**: Retrieve a list of available domain types
- **list_domains**: Retrieve a list of domains in Collibra
- **list_statuses**: Retrieve a list of available asset statuses
- **search_assets**: Search for assets by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Collibra** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all communities in Collibra."

**🤖 AI Agent:**
> You have 4 communities:
1. 'Data Governance' — 12 domains, 845 assets
2. 'Business Intelligence' — 8 domains, 532 assets
3. 'Compliance' — 5 domains, 210 assets
4. 'Engineering' — 15 domains, 1,204 assets
Would you like to explore domains in any of these?

---

**👤 You:**
> "Search for assets named 'Customer Data'."

**🤖 AI Agent:**
> 3 assets found matching 'Customer Data':
1. 'Customer Data Policy' (Data Policy) — Domain: Compliance
2. 'Customer Data Table' (Table) — Domain: Data Engineering
3. 'Customer Data Dictionary' (Business Term) — Domain: Data Governance
Would you like full details on any of these?

---

**👤 You:**
> "Who is the Data Steward assigned to the 'Product Inventory' asset?"

**🤖 AI Agent:**
> Querying asset 'Product Inventory'... The assigned Data Steward role belongs to Alice Smith (alice.smith@example.com) in the Data Governance community.


## ❓ FAQ

**Q: How do I authenticate with Collibra?**
This integration uses Basic Authentication with your Collibra instance URL, username, and password.

**Q: What is an asset in Collibra?**
An asset is any cataloged object: a business term, a database table, a column, a report, or a data policy, among others.

**Q: Can I create new communities or domains?**
The current version focuses on browsing metadata and creating assets. Community and domain creation may be added in future updates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/collibra](https://vinkius.com/mcp/collibra)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Collibra** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `collibra` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Collibra** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "collibra": {
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
