# ChurnZero MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/churnzero)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage customer success and health via ChurnZero — track churn scores, monitor segments, and analyze account activity directly from any AI agent.

## Description
Connect your **ChurnZero** account to any AI agent and take full control of your customer success operations through natural conversation. Streamline how you manage account health and retention workflows.

### What you can do

- **Account Oversight** — List and retrieve details for all customer accounts, including churn scores and health metrics natively
- **Contact Intelligence** — Access and monitor customer contact information and interaction history flawlessly
- **Event Tracking** — Log custom customer events and activities to refine health scoring securely
- **Communication Auditing** — List and review messages and automated communications sent to customers flawlessly
- **Success Logistics** — Monitor active playbooks and customer success journeys in real-time
- **Alert Visibility** — Access and review active success alerts to identify accounts needing immediate attention directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your ChurnZero App Key and instance App URL
3. Start managing your customer success from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Customer Success Managers** — monitor account health and review churn scores using natural language
- **Success Operations** — audit playbook performance and communication history without opening the dashboard
- **Sales Teams** — quickly look up account status and recent activities straight from their chat interface
- **Executives** — verify portfolio health and success journey progress


## Available Tools (8)
- **get_account_success_details**: Get detailed information for a specific account
- **list_churnzero_accounts**: List all customer accounts
- **list_churnzero_alerts**: List active customer success alerts
- **list_churnzero_contacts**: List all customer contacts
- **list_customer_journeys**: List active customer success journeys
- **list_customer_messages**: List messages and communications sent to customers
- **list_success_playbooks**: List active customer success playbooks
- **track_account_event**: Track a customer event or activity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ChurnZero** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the accounts with the highest churn risk."

**🤖 AI Agent:**
> Retrieving high-risk accounts... I found 3 accounts with health scores below 40: 'Global Tech', 'Fast Delivery', and 'Startup Inc'. Would you like to see their recent interaction history?

---

**👤 You:**
> "What are the latest customer success alerts?"

**🤖 AI Agent:**
> Checking active alerts... You have 5 new alerts today, including 2 'Low Usage' triggers and 3 'Key Contact Left' notifications. I can list the specific accounts for you.

---

**👤 You:**
> "Track a 'Feature Training Completed' event for account 'ACME-123'."

**🤖 AI Agent:**
> Tracking event for ACME-123... The 'Feature Training Completed' activity has been logged in ChurnZero. This will be factored into their health score during the next update.


## ❓ FAQ

**Q: Can I see the health score for a specific account?**
Yes! Use the `get_account_success_details` tool with the unique account External ID. The agent will return the churn score, health metrics, and current status from ChurnZero.

**Q: How do I check which success playbooks are currently active?**
Use the `list_success_playbooks` tool. Your agent will fetch all configured playbooks, allowing you to identify which automation flows are currently running.

**Q: Where do I find my ChurnZero App Key?**
Log in to ChurnZero, go to the **Admin** section, and look for **Application Keys**. You can generate a new App Key there for API access.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/churnzero](https://vinkius.com/mcp/churnzero)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ChurnZero** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `churnzero` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ChurnZero** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "churnzero": {
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
