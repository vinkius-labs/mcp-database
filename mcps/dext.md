# Dext MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dext)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage receipts, track invoices, and monitor accounting data via the Dext API.

## Description
Integrate **Dext** (formerly **Receipt Bank**), the leading bookkeeping and accounting automation platform, directly into your AI workflow. Manage your digital inbox of receipts and invoices, track supplier extraction data, and monitor accounting categories and client accounts using natural language.

### What you can do

- **Inbox Oversight** — List and retrieve detailed information for all items in your Dext inbox, including processing status.
- **Data Extraction** — Access granular technical metadata for extracted receipts, including tax details and supplier info.
- **Client Management** — List and review accounting clients and their integration settings in your partner account.
- **Account Intelligence** — Monitor connected bank accounts and accounting categories available for classification.

### How it works

1. Connect the Dext integration to your AI assistant.
2. Authorize using your Dext API Key (found in your account settings).
3. Optimize your bookkeeping and accounting operations through intuitive conversation.

### Who is this for?

- **Accountants & Bookkeepers** — Quickly check client inbox statuses and processing delays on the go.
- **Business Owners** — Monitor expense patterns and supplier extraction data via chat.
- **Finance Teams** — Audit accounting categories and tax rates during period-end closing.


## Available Tools (10)
- **get_account_metadata**: Retrieve metadata and usage limits for your Dext account
- **get_item_details**: Get detailed information for a specific inbox item
- **list_connected_bank_accounts**: List all bank accounts configured for statement extraction
- **list_accounting_categories**: List the chart of accounts or categories available for classification
- **list_accounting_clients**: List all clients associated with your Dext partner account
- **list_inbox_items**: List all pending and processed items (receipts, invoices) in your Dext inbox
- **list_extracted_suppliers**: List all suppliers automatically extracted from your documents
- **list_items_pending_review**: Identify inbox items that are currently in the "Review" status
- **list_account_users**: List all users with access to the current Dext account
- **search_inbox_by_keyword**: Search for receipts or invoices by supplier name or description


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dext** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all items in my inbox that need review."

**🤖 AI Agent:**
> I've found 5 items pending review, including a receipt from 'Staples' ($45.00) and an invoice from 'AWS' ($120.00). Would you like to see the tax breakdown for the AWS invoice?

---

**👤 You:**
> "Show me the details for the item from 'Starbucks' on June 12th."

**🤖 AI Agent:**
> I've retrieved the Starbucks receipt from June 12th. Total: $12.50. It has been categorized under 'Travel & Meals'. The extraction is 100% confident. Would you like the direct link to the document image?

---

**👤 You:**
> "Search my inbox for 'office supplies'."

**🤖 AI Agent:**
> I've found 3 items matching 'office supplies' from 'Office Depot' and 'Amazon'. The total spend across these items is $215.00. Should I list the individual dates and amounts?


## ❓ FAQ

**Q: How do I get a Dext API Key?**
Log in to your Dext account, navigate to **Settings > API**, and you can retrieve your unique API Key from that section. Ensure your plan includes API access.

**Q: Can the agent see receipt images?**
The agent can retrieve the URL for the item image, allowing you to click and view the original document directly from the chat interface.

**Q: Does the integration support multiple currencies?**
Yes, Dext automatically extracts the currency from your documents, and the agent will display the total amounts with their respective currency codes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dext](https://vinkius.com/mcp/dext)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dext** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dext` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dext** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dext": {
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
