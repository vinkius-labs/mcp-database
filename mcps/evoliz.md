# Evoliz MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/evoliz)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Handle French business invoicing with quote generation, expense tracking, and accounting integrations designed for compliance.

## Description
Connect your **Evoliz** account to any AI agent and take full control of your cloud invoicing and accounting workflows through natural conversation.

### What you can do

- **Invoicing Orchestration** — List and manage professional invoices programmatically, including retrieving detailed metadata and tracking payment statuses
- **Quote Management** — Programmatically fetch and list sales quotes to maintain a high-fidelity oversight of your pending deals
- **Client CRM** — Create and manage your complete customer database and retrieve detailed profiles directly through your agent
- **Catalog Intelligence** — Access your directory of articles (products/services) and retrieve technical metadata and pricing to coordinate sales
- **Accounting Visibility** — Monitor your business health by listing invoices and quotes programmatically using natural language commands

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** from your Evoliz settings (Settings > API)
3. Start managing your cloud accounting from Claude, Cursor, or any MCP client

No more manual deal logging or digging through fragmented accounting tables. Your AI acts as your dedicated accounting and billing coordinator.

### Who is this for?

- **SME Owners** — instantly check invoice statuses and client balances using natural language queries
- **Accountants & Ops** — monitor pending quotes and retrieve financial records without leaving your workspace
- **Sales Teams** — manage client profiles and coordinate article data through simple AI commands


## Available Tools
- **create_client**: Important required fields are usually `name` and `type` (Professional or Individual).

Create a new client in Evoliz
- **get_article**: Get a specific article in Evoliz
- **get_client**: Get a specific client in Evoliz
- **get_invoice**: Get a specific invoice in Evoliz
- **get_quote**: Get a specific quote in Evoliz
- **list_articles**: List articles (products/services) in Evoliz
- **list_clients**: List clients in Evoliz
- **list_invoices**: List invoices in Evoliz
- **list_quotes**: List quotes in Evoliz


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Evoliz** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my most recent invoices in Evoliz."

**🤖 AI Agent:**
> I've retrieved your latest invoices. You have 5 recent documents, including Invoice #INV-2026-01 (€450.00) and #INV-2026-02. Would you like to check the payment status for any of these?

---

**👤 You:**
> "Find the client named 'John Doe'."

**🤖 AI Agent:**
> Locating client... I've found John Doe's profile (ID: 12345). He is a 'Professional' client and has 3 past invoices with your company. Would you like to see his complete billing history?

---

**👤 You:**
> "Show me the details for quote ID '67890'."

**🤖 AI Agent:**
> Fetching quote 67890... This document is for 'Acme Corp' totaling €1,200.00. It includes 'Software Setup' and 'Training'. It is currently in 'Draft' status. Should I update the status to 'Sent'?


## ❓ FAQ

**Q: How do I find my Evoliz API Token?**
Log in to your account, navigate to **Settings** > **API**, and generate or copy your unique access token.

**Q: Does the agent send invoices automatically?**
No. The agent creates invoices as drafts. You must send them via the Evoliz interface or configure automation rules in your dashboard.

**Q: Can I check my product catalog via AI?**
Yes! Use the `list_articles` tool to retrieve your complete directory of products and services, including pricing and metadata.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/evoliz](https://vinkius.com/mcp/evoliz)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Evoliz** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `evoliz` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Evoliz** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "evoliz": {
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
