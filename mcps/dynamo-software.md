# Dynamo Software MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dynamo-software)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Equip your AI agent to manage alternative investments, track portfolios, and monitor funds via the Dynamo API.

## Description
Integrate **Dynamo Software**, the industry-leading platform for alternative investment management, directly into your AI workflow. Manage your investment funds and strategies, track investor profiles and commitment statuses, monitor portfolio valuations and activity logs, and oversee your entire investment lifecycle using natural language.

### What you can do

- **Fund Oversight** — List and retrieve detailed information, strategies, and performance metrics for all your investment funds.
- **Investor Intelligence** — Monitor registered investor profiles, unique identifiers, and current account statuses across your organization.
- **Portfolio Management** — Track investment portfolios, including associated asset counts and real-time valuation updates.
- **Activity Auditing** — Retrieve high-level summaries of recent activities, research notes, and engagement results instantly via chat.

### How it works

1. Connect the Dynamo Software integration to your AI assistant.
2. Authorize using your Dynamo API Key and Instance URL.
3. Orchestrate your investment management and portfolio optimization through intuitive conversation.

### Who is this for?

- **Investment Analysts** — Quickly check fund valuations and recent activity notes on the go.
- **Investor Relations** — Research investor profiles and commitment history via chat during outreach.
- **Portfolio Managers** — Monitor asset counts and organizational investment metadata instantly.


## Available Tools (10)
- **get_dynamo_account_metadata**: Retrieve metadata and usage limits for your Dynamo Software account
- **get_fund_details**: Get detailed settings and information for a specific investment fund
- **quick_portfolio_valuation_audit**: Retrieve a high-level summary of portfolio valuations and activity
- **list_active_investors_only**: Identify investors that are currently in an "Active" or "Funded" status
- **list_investment_funds**: List all investment funds managed in Dynamo
- **list_dynamo_investors**: List all investors registered in your Dynamo Software account
- **list_high_valuation_funds**: Identify funds with a valuation above a certain threshold (mock logic)
- **list_dynamo_portfolios**: List all investment portfolios configured in your account
- **list_latest_dynamo_activities**: Identify the most recently recorded activities and notes across the platform
- **search_investment_funds**: Search for funds using a name keyword or category


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dynamo Software** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active investors in our platform."

**🤖 AI Agent:**
> I've found several active investors, including 'Heritage Pension Fund' and 'Global Wealth Partners'. Both are currently 'Funded'. Would you like to see the last activity for Heritage Pension Fund?

---

**👤 You:**
> "Show me the top high-valuation investment funds."

**🤖 AI Agent:**
> The top funds by valuation are 'Growth Equity Fund IV' ($1.2B) and 'Global Infrastructure III' ($850M). Should I pull the performance metrics for Growth Equity Fund IV?

---

**👤 You:**
> "What are the most recent activities recorded in Dynamo?"

**🤖 AI Agent:**
> The latest activities include a 'Research Note' on Cloud Tech trends and an 'Investor Meeting' with Alice Smith. Both were recorded today. Would you like a summary of the Research Note?


## ❓ FAQ

**Q: How do I get a Dynamo Software API Key?**
Log in to your Dynamo Software instance, navigate to **User Settings** or **API Management**, and you can generate or retrieve your unique API Key from there. You will also need your specific Instance URL.

**Q: Can the agent update fund valuations?**
This integration currently focuses on listing and auditing investment data. Updating valuations or committed capital should be managed via the Dynamo Software web client or specific data import tools.

**Q: Does the integration support custom entities?**
Yes, while the core tools focus on investors and funds, the underlying engine is built to query common Dynamo entities. Custom entity support may vary based on your API configuration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dynamo-software](https://vinkius.com/mcp/dynamo-software)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dynamo Software** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dynamo-software` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dynamo Software** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dynamo-software": {
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
