# Chargeblast MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chargeblast)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Manage chargeback prevention and dispute alerts via Chargeblast — intercept disputes, automate refunds, and audit deflection logs directly from any AI agent.

## Description
Connect your **Chargeblast** account to any AI agent and take full control of your chargeback prevention and dispute management through natural conversation. Intercept disputes before they become chargebacks.

### What you can do

- **Alert Oversight** — List and retrieve details for all intercepted dispute alerts (CDRN, Ethoca, RDR) natively
- **Status Management** — Update alert statuses and mark disputes as refunded flawlessly
- **Deflection Auditing** — List and analyze logs of successfully blocked chargeback attempts securely
- **Order Logistics** — Upload order data to enable digital receipts and automatic deflections flawlessly
- **Merchant Enrollment** — List and manage enrolled merchants under your account in real-time
- **Credit Requests** — Trigger credit requests for specific dispute alerts directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Chargeblast API Key (obtained from Account Settings)
3. Start managing your chargeback alerts from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fraud Managers** — monitor intercepted alerts and review deflection history using natural language
- **E-commerce Operations** — automate refund processes for active alerts without opening the dashboard
- **Financial Controllers** — audit chargeback prevention success and credit requests straight from their chat interface
- **Platforms & Resellers** — manage multiple merchant enrollments and their alert statuses


## Available Tools (8)
- **request_dispute_credit**: Request a credit for a specific dispute alert
- **get_dispute_alert_details**: Get details for a specific dispute alert
- **list_dispute_alerts**: List all chargeback alerts from your account
- **list_deflection_logs**: List logs of chargeback attempts that were successfully blocked
- **list_enrolled_merchants**: List all merchants enrolled under your account
- **list_uploaded_orders**: List order history uploaded for deflection
- **update_alert_status**: Update the status of a dispute alert
- **upload_order_data**: Upload order data to enable digital receipts and deflections


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chargeblast** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all active dispute alerts in Chargeblast."

**🤖 AI Agent:**
> Retrieving your active alerts... I found 3 intercepted disputes: Alert #777 ($150.00 - Pending), #888 ($45.00 - Action Required), and #999 ($210.00 - Refunded).

---

**👤 You:**
> "What is the status of alert ID 12345?"

**🤖 AI Agent:**
> Checking alert 12345... This is an Ethoca alert for $99.99 from 'Jane Smith'. The current status is 'Awaiting Refund'. Would you like me to mark it as refunded now?

---

**👤 You:**
> "Show me the logs of chargebacks blocked today."

**🤖 AI Agent:**
> Retrieving today's deflection logs... Chargeblast successfully blocked 5 chargeback attempts today through automated RDR and digital receipt deflections, saving a total of $425.00.


## ❓ FAQ

**Q: Can I see my CDRN and Ethoca alerts in one place?**
Yes! Use the `list_dispute_alerts` tool. The agent will retrieve all intercepted alerts from various networks (CDRN, Ethoca, RDR) and display them in a unified list.

**Q: How do I mark an alert as refunded?**
Use the `update_alert_status` tool with the alert ID and set the status to `refunded`. This notifies Chargeblast that you have resolved the dispute manually.

**Q: Where do I find my Chargeblast API Key?**
Log in to your Chargeblast Dashboard and look for 'API Key' or 'Account Settings'. You can copy your key from that section for integration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chargeblast](https://vinkius.com/mcp/chargeblast)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chargeblast** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `chargeblast` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chargeblast** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chargeblast": {
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
