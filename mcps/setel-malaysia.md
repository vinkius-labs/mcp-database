# Setel Malaysia MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/setel-malaysia)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Orchestrate Setel Malaysia payments — manage payment intents, parking sessions, and EV charging directly from any AI agent.

## Description
Connect your AI agents to **Setel Malaysia**, the first e-wallet for fuel, parking, and on-the-go payments in Malaysia. This MCP provides 11 tools to automate payment orchestration, manage real-time parking sessions, and monitor EV charging infrastructure directly through natural conversation.

### What you can do

- **Payment Intent Flow** — Create, capture, and retrieve payment intents for secure transaction processing
- **Parking Management** — Start and monitor parking sessions for specific vehicle plates at automated or street locations
- **EV Mobility** — Find charging stations, start sessions, and end charging workflows programmatically
- **Loyalty Integration** — Check Mesra points balances for linked users to enhance customer engagement
- **Merchant Visibility** — Access account summaries and settlement data for business oversight

### How it works

1. Subscribe to this server
2. Register at the [**Setel Merchant Dashboard**](https://dashboard.setel.com/)
3. Navigate to **API Settings** to find your **API Key**, **API Secret**, and **Merchant ID**
4. Ensure you use the sandbox environment for initial testing
5. Insert your credentials into the fields below to start managing your mobility and payment workflows.

### Who is this for?

- **Fintech Developers** — automate the testing of payment flows and merchant reporting
- **Logistics & Fleet Managers** — monitor parking and fuel usage across multiple vehicles
- **Service Providers** — integrate Setel's EV charging and parking network into custom mobility apps smoothly


## Available Tools
- **capture_payment**: Capture an authorized payment
- **create_charging_session**: Start an EV charging session
- **create_parking_session**: Start a new parking session
- **create_payment_intent**: Returns a paymentIntentId for authorization.

Create a new payment intent for a transaction
- **end_charging_session**: Stop an active EV charging session
- **get_merchant_summary**: Get merchant account overview
- **get_mesra_points**: Retrieve loyalty points for a user
- **get_parking_session**: Retrieve details for an active or past parking session
- **get_payment_intent**: Retrieve details for a specific payment intent
- **list_charging_locations**: Find nearby EV charging stations
- **list_parking_history**: List recent parking sessions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Setel Malaysia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all Setel-compatible EV charging locations near me."

**🤖 AI Agent:**
> I'm searching the Setel charging network... I've found 3 nearby locations: 1. Petronas KLCC (ID: ev_101, Status: Available), 2. Suria Mall (ID: ev_102, Status: Busy), 3. Avenue K (ID: ev_103, Status: Available). Would you like the full connector details for any of these?

---

**👤 You:**
> "Check my Mesra points balance for user ID 'user_777'."

**🤖 AI Agent:**
> Retrieving loyalty data... User 'user_777' currently has 1,250 Mesra points. These can be redeemed for fuel discounts or retail rewards. Would you like to see available rewards?

---

**👤 You:**
> "Show the summary for my Setel merchant account."

**🤖 AI Agent:**
> Fetching merchant metrics... For April 2024, your total settlements amount to RM 45,200.00 across 1,200 transactions. Service status: All mobility services operational.


## ❓ FAQ

**Q: Can I test this in a staging environment?**
Yes! Setel provides a pre-production API (`api-pre-prod.setel.com`) for integration testing without affecting real balances.

**Q: How do I check the loyalty points for a user?**
Use the `get_mesra_points` tool with the specific User ID. Your agent will return the current Mesra points balance associated with that account.

**Q: Can I automatically list all nearby EV charging locations?**
Yes! The `list_charging_locations` tool retrieves available Setel-compatible EV chargers, allowing your agent to help you find the best spot to power up.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/setel-malaysia](https://vinkius.com/mcp/setel-malaysia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Setel Malaysia** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `setel-malaysia` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Setel Malaysia** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "setel-malaysia": {
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
