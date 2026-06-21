# Griffin MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/griffin)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage your banking & fintech operations via Griffin — list accounts, monitor transactions, and handle verifications via AI.

## Description
Connect your **Griffin** Banking-as-a-Service account to any AI agent and take full control of your embedded finance operations through natural conversation.

### What you can do

- **Index Orchestration** — Discover all available API resources and navigate your organization's banking infrastructure natively
- **Account Oversight** — List and inspect all bank accounts, including available balances and account numbers flawlessy
- **Live Transaction Monitoring** — Retrieve detailed transaction histories and resolve specific payment details including status and amounts flawlessly
- **Verification Workflow** — Manage KYC and KYB verifications by listing and inspecting individual verification records natively
- **Financial Transfers** — Trigger internal transfers between accounts to manage liquidity across your organization synchronously
- **Payee Management** — List and verify saved payees to ensure secure and accurate payment orchestration natively

### How it works

1. Subscribe to this server
2. Enter your Griffin API Key (found in your Griffin Dashboard under Settings > API keys)
3. Start managing your embedded banking operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fintech Operations Managers** — monitor real-time transaction flows and verify account balances via natural language
- **Compliance Officers** — audit KYC/KYB verification statuses and review individual verification details flawlessly
- **Product Engineers** — prototype banking features and verify API responses directly through the chat interface synchronously


## Available Tools
- **create_internal_transfer**: Transfer money between internal accounts
- **get_account**: Get details for a specific bank account
- **get_index**: Get the root index of resources from the Griffin API
- **get_me**: Get details of the current authenticated user
- **get_organization**: Get details for a specific organization
- **get_transaction**: Get details for a specific transaction
- **get_verification**: Get details for a specific verification
- **list_accounts**: List bank accounts for an organization
- **list_organizations**: List all accessible organizations
- **list_payees**: List saved payees for an organization
- **list_transactions**: Retrieve transaction history for a bank account
- **list_verifications**: List KYC/KYB verifications for an organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Griffin** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my organizations in Griffin"

**🤖 AI Agent:**
> Retrieving your organizations... I found 2 accessible organizations: 'Acme Corp' (ID: org_123) and 'Global Tech' (ID: org_456). Would you like to see the bank accounts for Acme Corp?

---

**👤 You:**
> "Show the recent transactions for account ID acc_93021"

**🤖 AI Agent:**
> Fetching transaction history... I found 3 recent payments for account acc_93021: 1. OUTBOUND: £150.00 (Status: Settled). 2. INBOUND: £1,200.00 (Status: Settled). 3. OUTBOUND: £45.50 (Status: Pending).

---

**👤 You:**
> "Check the KYC verification status for ID ver_88392"

**🤖 AI Agent:**
> Retrieving verification details... Verification ver_88392 for John Doe is currently 'Approved'. All identity and document checks have passed. Would you like to see the full decision metadata?


## ❓ FAQ

**Q: Can my agent list all bank accounts for a specific organization in Griffin?**
Yes. Use the 'list_accounts' tool with the 'organizationId' parameter. The agent will fetch all bank accounts associated with that organization flawlessly.

**Q: How do I check the status of a KYC/KYB verification via chat?**
You can use the 'get_verification' tool. Provide the Verification ID, and the agent will return the full details, including the current status and decision of the verification natively.

**Q: Can I trigger an internal money transfer between accounts through the agent?**
Absolutely. Use the 'create_internal_transfer' tool. By passing the amount and account IDs, your agent will programmatically trigger the transfer within Griffin's secure infrastructure flawlessly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/griffin](https://vinkius.com/mcp/griffin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Griffin** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `griffin` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Griffin** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "griffin": {
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
