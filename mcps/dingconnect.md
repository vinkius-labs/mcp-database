# DingConnect MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dingconnect)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Equip your AI agent to manage mobile top-ups, track operators, and monitor account balance via the DingConnect API.

## Description
Integrate **DingConnect**, the world's leading mobile top-up platform, directly into your AI workflow. Access thousands of mobile operators globally, manage your top-up and data products, monitor real-time account balances, and track transaction history using natural language.

### What you can do

- **Operator Discovery** — List and search for mobile network operators across 150+ countries supported by DingConnect.
- **Product Intelligence** — Access detailed information on available top-up and data plans, including technical keys and pricing.
- **Transaction Auditing** — List and retrieve detailed history for past service executions and their status.
- **Balance Management** — Track your account credit balance and organizational limits directly via chat.

### How it works

1. Connect the DingConnect integration to your AI assistant.
2. Authorize using your DingConnect API Key (found in your developer settings).
3. Orchestrate your global mobile services and top-ups through intuitive conversation.

### Who is this for?

- **Retail & Agent Managers** — Quickly check operator availability and product details on the go.
- **Finance Operations** — Monitor credit balances and transaction volumes via chat.
- **Customer Service Teams** — Research operator support and product offerings during customer resolution.


## Available Tools
- **check_mobile_service_status**: Check if mobile services are available for a specific destination (mock logic)
- **get_api_account_metadata**: Retrieve metadata and settings for your DingConnect API account
- **get_account_credit_balance**: Retrieve the current credit balance for your DingConnect account
- **quick_operator_audit**: Retrieve a high-level summary of operators and products for a country
- **list_supported_countries**: List all countries supported by DingConnect for mobile services
- **list_transaction_history**: List recent top-up transactions and service history
- **list_top_volume_countries**: Identify countries with high service availability (mock logic)
- **list_available_topup_products**: List all available top-up and data products for a specific provider
- **list_mobile_operators**: List all mobile network operators (providers) for a specific country
- **search_topup_products**: Search for specific top-up or data products by name keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DingConnect** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all mobile operators available in Brazil."

**🤖 AI Agent:**
> I've found 4 operators available in Brazil via DingConnect: 'Vivo', 'Claro', 'TIM', and 'Oi'. Would you like to see the available top-up products for Vivo?

---

**👤 You:**
> "What is my current account credit balance?"

**🤖 AI Agent:**
> Your current account balance is $250.45 USD. You have successfully processed 15 transactions today. Should I show you the recent transaction history?

---

**👤 You:**
> "Show me the top-up plans for operator 'Safaricom' in Kenya."

**🤖 AI Agent:**
> For Safaricom Kenya (KE), I've found several plans including '100 KES Top-up', '500MB Data Bundle', and 'International Voice Package'. Would you like the technical product keys for any of these?


## ❓ FAQ

**Q: How do I get a DingConnect API Key?**
Log in to your DingConnect account and navigate to the developer portal or API settings section to generate or retrieve your unique API Key.

**Q: Can the agent perform actual top-ups?**
This integration currently focuses on discovering operators, products, and auditing balance and history. Executing actual financial top-ups should be managed via the DingConnect portal or specialized integration.

**Q: Does the integration show real-time exchange rates?**
Yes, when retrieving product pricing, the agent provides the latest rates and currency conversions as reported by the DingConnect platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dingconnect](https://vinkius.com/mcp/dingconnect)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DingConnect** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `dingconnect` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DingConnect** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dingconnect": {
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
