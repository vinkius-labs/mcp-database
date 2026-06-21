# Avalara (AvaTax) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/avalara-avatax)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate tax calculation and compliance with Avalara AvaTax — calculate rates and resolve addresses via AI.

## Description
Connect your **Avalara AvaTax** account to any AI agent and automate your transaction tax compliance through natural conversation.

### What you can do

- **Real-time Tax Calculation** — Create and record transactions with accurate sales tax rates for any global jurisdiction
- **Precision Address Validation** — Resolve and validate physical addresses to ensure maximum calculation accuracy and nexus compliance
- **Seamless Transaction Management** — Retrieve, commit, and void tax transactions directly from your chat interface
- **Compliance & Nexus Auditing** — List tax nexus settings and company details to ensure your business remains compliant with local regulations

### How it works

1. Subscribe to this server
2. Enter your AvaTax Username (Account ID) and Password (License Key)
3. Start managing your tax compliance from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance & Accounting Teams** — instantly calculate taxes for complex orders and audit company nexus settings
- **E-commerce Operations** — validate shipping addresses and ensure tax compliance without manual data entry
- **Developers** — test tax calculation logic in sandbox and audit transaction records through natural language commands


## Available Tools (10)
- **commit_transaction**: Mark a transaction as committed for reporting
- **create_transaction**: Calculate tax and record a transaction
- **get_account_check**: Verify AvaTax account connection
- **get_company**: Get details for a specific company
- **get_tax_rates_by_address**: Get tax rates for a physical address
- **get_transaction**: Retrieve a specific transaction by code
- **list_companies**: List all companies in the account
- **list_nexus**: List tax nexus for a specific company
- **resolve_address**: Validate and resolve a physical address
- **void_transaction**: Void a transaction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Avalara (AvaTax)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Resolve the following address: '2000 Main St, Irvine, CA 92614'."

**🤖 AI Agent:**
> I've resolved the address. It is a valid physical location: 2000 Main St, Irvine, CA, 92614-7223, US. The jurisdiction codes have been identified for accurate tax calculation. Shall I proceed with a tax quote for this location?

---

**👤 You:**
> "List all active nexus settings for my company 'MainStore'."

**🤖 AI Agent:**
> I've retrieved the nexus list for 'MainStore'. You currently have active tax obligations in 5 jurisdictions, including California, New York, and Texas. Would you like to see the specific effective dates for each?

---

**👤 You:**
> "Calculate sales tax for a $100.00 purchase from Seattle to New York."

**🤖 AI Agent:**
> Based on the origin (Seattle) and destination (New York), the total sales tax for a $100.00 purchase is $8.88. This includes the state, city, and special district taxes. Would you like me to record this transaction in your AvaTax ledger?


## ❓ FAQ

**Q: Can the AI automatically validate a shipping address before I calculate the tax?**
Yes! Use the `resolve_address` tool with the full address string. Your agent will return the validated and formatted address, ensuring that the subsequent tax calculation uses the correct jurisdiction data.

**Q: How do I void a transaction that was recorded incorrectly?**
Simply ask the agent to run the `void_transaction` tool with the specific transaction code and company code. It will instantly update the status in your AvaTax account.

**Q: Is it possible to check my company's tax nexus settings through the AI?**
Yes. The `list_nexus_by_company` tool allows you to audit all active tax jurisdictions where your company is registered, ensuring you are collecting taxes where required.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/avalara-avatax](https://vinkius.com/mcp/avalara-avatax)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Avalara (AvaTax)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `avalara-avatax` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Avalara (AvaTax)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "avalara-avatax": {
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
