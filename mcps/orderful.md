# Orderful MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/orderful)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics-supply-chain](../categories/logistics-supply-chain.md)

EDI integration made simple — manage transactions, relationships, and guidelines via Orderful.

## Description
Connect your **Orderful** account to empower your AI agents with modern EDI capabilities. This server provides programmatic access to the Orderful V3 API for managing B2B supply chain transactions and trading partner relationships.

### What you can do

- **Transaction Monitoring** — List and inspect inbound and outbound EDI transactions in real-time
- **Error Diagnosis** — Retrieve validation and processing errors for specific transactions
- **Relationship Management** — Monitor active trading partner relationships and identifiers
- **Infrastructure Visibility** — Access communication channels, guidelines, and supported transaction types
- **Supply Chain Orchestration** — Automate EDI lookups and status checks through simple natural language commands

### How it works

1. Subscribe to this server
2. Enter your **Orderful API Key** from your settings panel
3. Start managing your EDI operations from Claude, Cursor, or any MCP client


## Available Tools
- **get_organization**: Get organization details
- **get_transaction**: Get details for a specific transaction
- **get_transaction_errors**: Get errors for a transaction
- **list_communication_channels**: List communication channels
- **list_guidelines**: List EDI guidelines
- **list_relationships**: List trading partner relationships
- **list_transaction_types**: List supported transaction types
- **list_transactions**: List EDI transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Orderful** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my recent EDI transactions."

**🤖 AI Agent:**
> Fetching transactions... I've found 12 recent EDI exchanges. 8 are RECEIVED and 4 were SENT successfully.


## ❓ FAQ

**Q: How do I find my Orderful API Key?**
Log in to Orderful, click your User Icon > Settings, and look for API Credentials under Organization Settings.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/orderful](https://vinkius.com/mcp/orderful)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Orderful** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `orderful` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Orderful** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "orderful": {
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
