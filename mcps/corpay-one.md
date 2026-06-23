# Corpay One MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/corpay-one)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Simplify business payments with automated AP processing, virtual cards, and vendor management that saves your finance team hours.

## Description
Connect your **Corpay One** business payment account to any AI agent and simplify how you pay bills, manage vendor relationships, and monitor your financial documents through natural conversation.

### What you can do

- **Payment Oversight** — List all processed and scheduled bill payments and retrieve detailed reconciliation metadata.
- **Document Management** — Query your catalog of scanned or uploaded invoices and receipts with full data extraction details.
- **Vendor CRM** — List all registered vendors and suppliers to manage your procurement network effectively.
- **Financial Insights** — Check the real-time status of individual payments and documents directly from the agent.
- **Team Coordination** — List account users and team members to understand organizational distribution.
- **Workflow Automation** — Upload new document metadata and initiate financial records via AI commands.

### How it works

1. Subscribe to this server
2. Enter your Corpay One API Key (found in your account settings under API)
3. Start managing your business payments from Claude, Cursor, or any MCP client

### Who is this for?

- **Finance Managers & Controllers** — quickly check payment statuses and verify invoice data via simple AI queries.
- **Accounts Payable Teams** — monitor vendor directories and track document approval flows directly from the workspace.
- **Business Owners** — get instant bird's-eye views of company spending and upcoming bill payments via the AI assistant.


## Available Tools (7)
- **create_new_document**: Upload a new document
- **get_document_details**: Get details for a specific document
- **get_payment_details**: Get details for a specific payment
- **list_financial_documents**: List invoices and receipts
- **list_payments**: List Corpay One payments
- **list_team_users**: List account users
- **list_account_vendors**: List vendors/suppliers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Corpay One** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my recent bill payments."

**🤖 AI Agent:**
> I've retrieved your payments history. You have 3 recent payments including #PAY-10293 ($1,250.00 to AWS), #PAY-10294 ($450.00 to Staples), and 1 scheduled payment. Which one would you like more details on?

---

**👤 You:**
> "Show me the details for invoice 'doc_88231'."

**🤖 AI Agent:**
> Fetching document... Invoice doc_88231 is from 'Cloud Solutions Ltd' for the amount of $2,400.00 USD. It was uploaded on Dec 1st and is currently 'Awaiting Approval'. Would you like the full breakdown?

---

**👤 You:**
> "List all vendors in my account."

**🤖 AI Agent:**
> Retrieving vendors... You have 15 registered suppliers including 'Amazon Business', 'Google Cloud', 'Local Office Supplies', and 'Utility Co'. Shall I check the latest payments for any specific vendor?


## ❓ FAQ

**Q: Can I check the status of a specific bill payment via AI?**
Yes! Use the `get_payment_details` tool and provide the Payment ID. Your agent will retrieve the current status, amount, and reconciliation data.

**Q: How do I list all the vendors registered in my account?**
Run the `list_account_vendors` query. The agent will retrieve the complete list of suppliers and vendors currently configured in your Corpay One account.

**Q: Is it possible to see the details of a scanned invoice via AI?**
Absolutely. Use the `get_document_details` tool with your Document ID. Your agent will return the extracted metadata, including vendor name, total amount, and due date.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/corpay-one](https://vinkius.com/mcp/corpay-one)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Corpay One** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `corpay-one` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Corpay One** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "corpay-one": {
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
