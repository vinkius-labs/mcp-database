# Churnkey MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/churnkey)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Manage customer retention and cancellation flows via Churnkey — track sessions, analyze exit surveys, and automate recovery contacts directly from any AI agent.

## Description
Connect your **Churnkey** account to any AI agent and take full control of your customer retention and cancellation automation through natural conversation. Streamline how you handle churn and recover failed payments.

### What you can do

- **Session Oversight** — List and retrieve details for all customer cancellation flow sessions natively
- **Aggregation Intelligence** — Access grouped session counts to identify trends in churn reasons flawlessly
- **Recovery Logistics** — Update and manage billing recovery contacts for specific customers securely
- **Retention Deep-Dives** — List all cancellation sessions for a specific customer to understand their history flawlessly
- **Compliance Management** — Access and delete customer data for GDPR requests directly within your workspace flawlessly
- **Data Logistics** — Retrieve session metadata including offer types (discounts, pauses) and billing intervals flawlessly

### How it works

1. Subscribe to this server
2. Enter your Churnkey Data API Key and App ID (obtained from Settings > Account)
3. Start managing your retention flows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SaaS Founders** — monitor churn reasons and retention success rates using natural language
- **Customer Success Managers** — review specific cancellation sessions without opening the dashboard
- **Finance Teams** — manage billing recovery contacts and monitor saved revenue straight from their chat interface
- **Operations Teams** — verify GDPR data access and deletion requests


## Available Tools
- **bulk_update_billing_contacts**: Update billing recovery contacts for multiple customers at once
- **delete_customer_gdpr_data**: Delete all data for a customer for GDPR compliance
- **get_session_aggregates**: Retrieve grouped session counts
- **list_customer_retention_history**: List all cancellation sessions for a specific customer
- **get_customer_gdpr_data**: Access all data stored for a customer for GDPR compliance
- **get_retention_session_details**: Get details for a specific cancellation session
- **list_retention_sessions**: List cancellation flow sessions
- **update_billing_contacts**: Update recovery contacts for a specific customer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Churnkey** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the last 5 cancellation sessions in Churnkey."

**🤖 AI Agent:**
> Retrieving recent sessions... I found 5 sessions. 3 users were retained with a 'Pause' offer, 1 accepted a '50% Discount', and 1 proceeded to cancel. Would you like to see the reasons they provided?

---

**👤 You:**
> "What are the session aggregates for this month?"

**🤖 AI Agent:**
> Analyzing session data... This month you had 150 cancellation attempts. Your retention rate is 45%, with 'Price' being the top reason for leaving (60% of sessions).

---

**👤 You:**
> "List all retention sessions for customer 'cust_123'."

**🤖 AI Agent:**
> Checking history for cust_123... I found 2 sessions. In January they accepted a '3 month pause', and yesterday they proceeded with the cancellation due to 'Product complexity'.


## ❓ FAQ

**Q: Can I see the most common reason users are trying to cancel?**
Yes! Use the `get_session_aggregates` tool. The agent will return grouped data showing which reasons are being selected most frequently in your cancellation flows.

**Q: How do I update the billing contact for a customer whose payment failed?**
Use the `update_billing_contacts` tool. Provide the customer ID and the new contact details. This ensures Churnkey sends dunning and recovery emails to the right person.

**Q: Where do I find my Churnkey Data API Key and App ID?**
Log in to your Churnkey dashboard and navigate to **Settings > Account**. You can find your App ID and generate a Data API Key in the API section.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/churnkey](https://vinkius.com/mcp/churnkey)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Churnkey** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `churnkey` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Churnkey** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "churnkey": {
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
