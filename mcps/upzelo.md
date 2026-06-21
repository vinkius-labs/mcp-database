# Upzelo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/upzelo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Reduce subscription churn with personalized retention offers that intercept cancellations and win back customers at the exit point.

## Description
Connect your **Upzelo** churn management account to any AI agent and simplify how you retain customers and manage subscription lifecycles through natural conversation.

### What you can do

- **Customer Management** — List and search customer records, and update profile data for better segmentation and targeting.
- **Retention Flows** — List available flows and manually trigger retention sequences for customers at risk of cancelling.
- **Subscription Tracking** — Query all tracked subscriptions and update statuses or trial details programmatically.
- **Flow Monitoring** — Check the real-time status and outcomes of active flow sessions to verify retention success.
- **External ID Sync** — Link your internal system identifiers to Upzelo customer records for seamless integration.

### How it works

1. Subscribe to this server
2. Enter your Upzelo App ID and API Key (found in your developer settings)
3. Start managing your retention strategy from Claude, Cursor, or any MCP client

### Who is this for?

- **Customer Success Managers** — quickly trigger retention flows and check customer health via simple AI commands.
- **Product Operations** — monitor subscription statuses and sync customer data directly from the workspace.
- **Business Growth Teams** — get instant insights into flow performance and active retention sessions.


## Available Tools
- **save_customer**: Used for segmentation and targeting.

Create or update a customer record
- **get_customer**: Get details for a specific customer
- **get_flow_session**: Check the status of a flow session
- **get_flow**: Get details for a specific flow
- **get_subscription**: Get details for a specific subscription
- **list_customers**: List all customers in Upzelo
- **list_flows**: List all retention flows
- **list_subscriptions**: List all subscriptions
- **start_flow**: Initialize a flow for a customer
- **update_subscription**: Update subscription attributes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Upzelo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all customers currently tracked in Upzelo."

**🤖 AI Agent:**
> I've retrieved your customer list. You have 25 active profiles including 'John Miller', 'Sarah Smith', and 'Global Tech'. Would you like to check the retention status for any of them?

---

**👤 You:**
> "Trigger the 'Basic Retention' flow (ID: fl_8823) for customer 'cust_1029'."

**🤖 AI Agent:**
> Retention flow initialized! I've started the 'Basic Retention' sequence for customer cust_1029. The session ID is sess_99023. I'll monitor for the final outcome.

---

**👤 You:**
> "Show me the details for subscription 'sub_12903'."

**🤖 AI Agent:**
> Fetching subscription data... Subscription sub_12903 is currently 'Active'. It's on the 'Professional Plan' and the next renewal is scheduled for Dec 15th. Shall I update any attributes?


## ❓ FAQ

**Q: Can I manually start a retention flow for a customer via AI?**
Yes! Use the `start_flow` tool and provide the Flow ID, Customer ID, and Subscription ID. This will initialize the retention experience for that user immediately.

**Q: How do I see if a customer successfully stayed after a flow?**
Run the `get_flow_session` query with the specific Session ID. It will return the outcome and status of the retention attempt.

**Q: Is it possible to update a subscription's status via AI?**
Absolutely. Use the `update_subscription` tool by providing the Subscription ID and the new status to synchronize data between your systems and Upzelo.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/upzelo](https://vinkius.com/mcp/upzelo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Upzelo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `upzelo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Upzelo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "upzelo": {
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
