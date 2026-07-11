# Delio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/delio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [compliance](../categories/compliance.md)

Automate wealth management workflows via Delio Core OS — manage deals, investors, portfolio transactions, compliance forms, and platform users from any AI agent.

## Description
Connect your **Delio Core OS** tenant to any AI agent and take full control of your private markets wealth management workflows through natural conversation.

### What you can do

- **Deal Lifecycle** — Check deal workflow status, list investor workflows per deal, and browse all transactions across deals
- **Portfolio Management** — List and inspect assets (direct investments and PE funds), investors, and the full transaction lifecycle (subscriptions, capital calls, distributions, fees)
- **User Management** — List and search platform users, fetch a user’s full data graph, invite new users, and browse user groups
- **Compliance** — List compliance form definitions (KYC, AML, investor classification) and retrieve individual compliance implementations with submitted answers
- **Organisation Settings** — Read tenant-level configuration as a key/value map

### How it works

1. Subscribe to this server
2. Enter your Delio API Token and tenant Base URL
3. Start managing deals, portfolio, users, and compliance from Claude, Cursor, or any MCP-compatible client

Your AI acts as a dedicated wealth management operations assistant — no more switching between the Delio portal and your editor to check a deal status or look up an investor.

### Who is this for?

- **Investment Managers** — check deal progress, browse portfolio assets and investors, and track transactions without leaving the conversation
- **Operations Teams** — invite users, manage compliance forms, and read organisation settings directly from your AI agent
- **Integration Engineers** — use the MCP as a live API explorer to understand Delio’s data model before building deeper integrations


## Available Tools (14)
- **list_deal_investor_workflows**: List investor workflows for a deal
- **list_deal_transactions**: Includes subscriptions, capital calls, distributions, fees, and adjustments.

List all transactions across deals
- **get_deal_workflow_status**: Shows where the investor is in the lifecycle from invitation to completed transaction.

Get deal workflow status
- **get_asset_details**: Get detailed information about a specific asset
- **get_compliance_implementation**: Get a compliance implementation with submitted answers
- **get_user**: Get a single user with their full data graph
- **invite_user**: The body should include email, name, user type, and any required group or role assignments.

Send a platform invitation to a new user
- **list_portfolio_assets**: List all portfolio assets
- **list_compliance_forms**: List all compliance form definitions
- **list_portfolio_investors**: List all portfolio investors
- **list_organisation_settings**: List tenant organisation settings
- **list_portfolio_transactions**: List all portfolio transactions
- **list_user_groups**: List all user groups in the tenant
- **list_users**: Supports search by name or email, sorting, and pagination.

List all platform users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Delio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all users in our Delio tenant, searching for 'john'."

**🤖 AI Agent:**
> Found 2 users matching 'john': John Smith (john@acme.com, UUID: a1b2c3) and Jonathan Lee (jlee@acme.com, UUID: d4e5f6). Both are active investors. Would you like the full data graph for either?

---

**👤 You:**
> "What is the current workflow status for deal deal-456?"

**🤖 AI Agent:**
> Deal deal-456 is currently at the 'KYC Verification' step. There are no blocking conditions — the investor can proceed to the next step. Two investor workflows are attached to this deal.

---

**👤 You:**
> "Show me all portfolio assets, page 1 with 20 per page."

**🤖 AI Agent:**
> Retrieved 20 assets on page 1. Notable holdings include: 'Acme Growth Fund I' (PE Fund, ID: 101), 'TechDirect Holdings' (Direct Investment, ID: 102), and 'Real Estate Portfolio A' (Direct Investment, ID: 103). Would you like details on any specific asset?


## ❓ FAQ

**Q: How do I get a Delio API token?**
API tokens are issued by the Delio team. Contact your Delio integration lead and tell them your tenant name, whether you need sandbox or production, and the team or system that will hold the token. Tokens are bearer credentials — treat them like passwords and cycle them regularly via the Token API.

**Q: What is the difference between sandbox and production?**
Every tenant has two environments: sandbox (isolated data, safe for development and testing, URLs like `https://<tenant>.sandbox.deliowealth.com/`) and production (your live tenant, URLs like `https://<tenant>.deliowealth.com/`). The API surface is identical — build against sandbox, then switch the base URL when ready.

**Q: Can my AI manage the full deal lifecycle?**
Yes. Use `get_deal_workflow_status` to check where an investor is in the deal lifecycle, `list_deal_investor_workflows` to see every investor's progress on a deal, and `list_deal_transactions` to browse all transactions across deals. This gives your AI full visibility into the deal pipeline from invitation to completed transaction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/delio](https://vinkius.com/mcp/delio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Delio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `delio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Delio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "delio": {
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
