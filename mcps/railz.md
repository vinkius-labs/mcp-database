# Railz MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/railz)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Financial data integration platform — connect accounting, banking, and commerce data via AI.

## Description
Empower your AI agent to access normalized financial data from various accounting, banking, and commerce platforms with **Railz**. By connecting Railz to your agent, you transform complex financial auditing into a natural conversation. Your agent can instantly list businesses, audit invoices, and retrieve deep financial reports like Balance Sheets and P&L statements without you ever touching a dashboard. Whether you are managing multiple client accounts or a single corporate entity, your agent acts as a real-time financial analyst, ensuring your data is always accessible and structured.

### What you can do

- **Business Directory** — List all registered businesses in your Railz account and inspect their specific metadata.
- **Connection Auditing** — Monitor active service provider connections (QuickBooks, Xero, Shopify, etc.) for any business entity.
- **Financial Reporting** — Fetch real-time, normalized reports including Balance Sheets, Profit & Loss, and Cash Flow statements.
- **Invoice & Bill Management** — Query and analyze accounts receivable (invoices) and accounts payable (bills) across multiple providers.
- **Commerce Insights** — Access sales orders and transaction data from connected commerce platforms to track revenue trends.

### How it works

1. Subscribe to this server
2. Enter your Railz Client ID and Client Secret
3. Start managing your financial data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Accountants & Bookkeepers** — instantly retrieve financial statements and audit transactions across different client accounting systems.
- **Financial Analysts** — perform rapid health checks on business revenue and cash flow without manual data exports.
- **SaaS Developers** — integrate financial data workflows into your applications through an AI-guided interface.
- **Business Owners** — monitor your company's financial health and commerce orders through simple natural language queries.


## Available Tools (12)
- **get_balance_sheet**: Get balance sheet report
- **list_bank_transactions**: List bank transactions
- **get_cash_flow**: Get cash flow statement
- **list_commerce_orders**: g., Shopify, BigCommerce).

List commerce orders
- **get_business**: Get details for a specific business
- **list_journal_entries**: List journal entries
- **list_accounts**: List chart of accounts
- **list_bills**: List bills for a business
- **list_businesses**: List all businesses in Railz
- **list_connections**: g., QuickBooks, Xero) for a given business.

List connections for a business
- **list_invoices**: List invoices for a business
- **get_profit_and_loss**: Get profit and loss report


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Railz** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all businesses registered in my Railz account."

**🤖 AI Agent:**
> I've retrieved your business directory. You currently have 3 registered entities: 'Acme Corp', 'Global Logistics', and 'Retail Ventures'. Which one would you like to inspect?

---

**👤 You:**
> "Show active connections for business 'biz_123'."

**🤖 AI Agent:**
> Business 'biz_123' has 2 active connections: 'QuickBooks Online' (conn_456) and 'Shopify' (conn_789). I can now pull reports or transaction data from either source.

---

**👤 You:**
> "Get the Profit and Loss report for connection 'conn_456'."

**🤖 AI Agent:**
> Fetching normalized P&L data... For the current period, your total revenue is $50,000 with operating expenses of $30,000, resulting in a net income of $20,000.


## ❓ FAQ

**Q: Can I access data from multiple accounting platforms like QuickBooks and Xero simultaneously?**
Yes! Railz normalizes data across all supported providers. Use the `list_businesses` and `list_connections` tools to identify the target entity, then query reports which will return in a consistent format regardless of the underlying source.

**Q: How do I retrieve a Balance Sheet for a specific company connection?**
First, find the relevant `connection_id` for the business using `list_connections`. Then, use the `get_balance_sheet` tool with that ID to fetch the snapshot of assets and liabilities.

**Q: Does this integration allow creating new invoices or only reading them?**
The current toolset focuses on read-only operations for auditing and analysis, such as `list_invoices`, `list_bills`, and `list_accounts`. This ensures safe exploration of financial data without accidental modifications.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/railz](https://vinkius.com/mcp/railz)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Railz** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `railz` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Railz** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "railz": {
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
