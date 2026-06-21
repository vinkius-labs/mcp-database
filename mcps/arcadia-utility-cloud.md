# Arcadia Utility Cloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arcadia-utility-cloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Automate utility data collection with Arcadia Utility Cloud — track accounts, bills, and usage via AI.

## Description
The **Arcadia Utility Cloud MCP Server** (formerly Urjanet) provides an advanced natural language interface for automated utility data management. Seamlessly retrieve billing data, monitor consumption patterns, and audit your utility account inventory across thousands of global providers.

### Key Capabilities

- **Automated Statement Collection** — List and retrieve metadata for all collected utility bills, including charges and periods.
- **Consumption Monitoring** — Access granular usage data for individual meters to analyze energy and resource patterns.
- **Inventory Oversight** — Manage your large-scale inventory of utility accounts and meters with ease.
- **Global Provider Support** — Interface with a vast network of electric, gas, water, and waste providers through a unified API.
- **Data Integrity** — Access verified, high-quality utility data suitable for financial and sustainability reporting.
- **Secure Integration** — Uses standard OAuth 2.0 authentication to protect your sensitive operational data.

### Who is this for?

- **Sustainability Managers** — Effortlessly gather utility data for carbon footprint calculations and ESG disclosures.
- **Accounts Payable** — Audit utility billing across large portfolios to ensure accuracy and identify savings.
- **Energy Engineers** — Retrieve meter-level data to monitor efficiency improvements and resource consumption.


## Available Tools
- **get_account_check**: Verify Arcadia Utility Cloud connection
- **get_meter_data**: Retrieve consumption and usage data for a specific meter
- **get_statement**: Get metadata for a specific statement
- **list_accounts**: List all utility accounts available in the Utility Cloud
- **list_meters**: List all utility meters tracked in the cloud
- **list_statements**: List all collected utility statements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Arcadia Utility Cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active utility accounts in the cloud."

**🤖 AI Agent:**
> I've retrieved your active inventory. You have 25 accounts across 5 providers, including electricity, water, and gas services.

---

**👤 You:**
> "Get consumption data for water meter 'met_12345'."

**🤖 AI Agent:**
> Retrieved usage data for meter 'met_12345'. In the last billing period, it recorded 4,500 gallons of water consumption.

---

**👤 You:**
> "Show me the latest electricity bill metadata for account ID 'acc_9988'."

**🤖 AI Agent:**
> The latest statement for account 'acc_9988' was issued on Jan 15, 2024, with total charges of $312.50.


## ❓ FAQ

**Q: How do I get my Arcadia Utility Cloud credentials?**
You can generate API Client credentials in the [Arcadia Dashboard](https://dashboard.arcadia.com/). These credentials provide access to the Utility Cloud (formerly Urjanet) datasets.

**Q: Is consumption data available for all meters?**
Yes, basic consumption data is available via the `get_meter_data` tool for any meter successfully linked and scraped by the Arcadia platform.

**Q: Does this replace the Arcadia Plug server?**
This server specifically targets Utility Cloud (historical and aggregate bill data), while Arcadia Plug is designed for real-time account linking and higher-resolution data. They can be used together.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arcadia-utility-cloud](https://vinkius.com/mcp/arcadia-utility-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Arcadia Utility Cloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `arcadia-utility-cloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Arcadia Utility Cloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "arcadia-utility-cloud": {
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
