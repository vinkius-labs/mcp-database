# Skalin MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/skalin)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage accounts, contacts, and customer health on Skalin with AI agents.

## Description
Connect your **Skalin** account to any AI agent to automate your customer success and account management operations. Skalin provides a premier platform for monitoring customer health, tracking interactions, and managing tasks, and this integration allows you to retrieve account metadata, monitor health scores, and track alerts through natural conversation.

### What you can do

- **Account & CRM Orchestration** — List all managed accounts and retrieve detailed profile metadata, including status and owner info programmatically.
- **Customer Health Monitoring** — Access real-time health scores and metrics for your accounts to identify churn risks directly from the AI interface.
- **Interaction Lifecycle Management** — Create and monitor customer interactions and tasks to ensure your team's workflow is always synchronized.
- **Alert & Notification Control** — List and monitor system alerts to stay on top of critical account changes via natural language.
- **Team Coordination** — Access and monitor CSM assignments and task progress to ensure optimal customer coverage.

### How it works

1. Subscribe to this server
2. Enter your Skalin API Key from your integration settings
3. Start managing your customer success from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Customer Success Managers** — quickly retrieve account health and interaction history without switching apps.
- **Account Executives** — automate the retrieval of client details and monitor recent alerts via natural conversation.
- **Operations Teams** — streamline the retrieval of account metrics and manage team tasks directly within the chat.


## Available Tools (12)
- **get_account_metrics**: Get usage metrics
- **list_cs_accounts**: List customer accounts
- **list_cs_alerts**: ).

Get active alerts
- **list_account_contacts**: List account people
- **list_success_managers**: List CSM users
- **list_account_interactions**: Get account history
- **list_cs_tasks**: List success tasks
- **update_cs_task**: Modify success task
- **create_cs_account**: Add new account
- **log_interaction**: Record meeting or email
- **get_api_status**: Get connectivity info
- **get_account_health**: Check client health


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Skalin** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all accounts with a health score below 50 in Skalin."

**🤖 AI Agent:**
> I've retrieved the at-risk accounts. You have 3 accounts with health scores below 50: 'Acme Corp' (35), 'Globex Inc' (42), and 'Initech' (48). Would you like to see recent alerts for any of them?

---

**👤 You:**
> "Show me the customer health scores for all enterprise accounts with churn risk indicators."

**🤖 AI Agent:**
> 34 enterprise accounts analyzed. Healthy (22, 65%): Avg health score 87, strong product adoption, regular engagement. At-risk (8, 24%): Avg score 52. Top concerns: Meridian Corp (score 38, login drop 67%), TechVentures (score 45, support tickets +200%), DataFlow (score 51, feature adoption 12%). Churning (4, 12%): 2 confirmed non-renewal, 2 in negotiation. Net Revenue Retention: 108%. Key risk signals: declining logins (5 accounts), reduced feature usage (3), negative NPS (2). CSM action items: 12 tasks overdue.

---

**👤 You:**
> "Generate a quarterly business review report for the Meridian Corp account."

**🤖 AI Agent:**
> QBR Report: Meridian Corp (Q1 2025). Health score: 38/100 (Critical). Contract value: $180,000/year (renewal: August 15). Usage: 45 active users of 100 licenses (45% adoption, down from 67%). Feature adoption: 4 of 12 modules active. Support: 23 tickets (vs 8 last quarter, +188%). NPS: 6 (Passive, was 8). Key wins: API integration completed, custom dashboard deployed. Concerns: Champions left the company (2), executive sponsor unresponsive. Recommended actions: Executive alignment meeting, adoption workshop, contract review.


## ❓ FAQ

**Q: How do I find my Skalin API Key?**
Log in to your Skalin account, navigate to **Settings** > **Integrations**, and you will find your unique secret API Bearer Token there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/skalin](https://vinkius.com/mcp/skalin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Skalin** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `skalin` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Skalin** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "skalin": {
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
