# Jitbit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jitbit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track and resolve IT support tickets with a fast helpdesk that includes automation rules, knowledge base, and SLA monitoring.

## Description
Connect your **Jitbit** instance to any AI agent and manage your helpdesk through natural conversation.

### What you can do

- **Ticket Management** — List tickets, inspect details, create new tickets, and update status
- **Assignment Tracking** — Monitor agent assignments and workload
- **Category Browsing** — Navigate ticket categories for organized support
- **Response Management** — Reply to tickets and add internal notes
- **SLA Monitoring** — Track response and resolution time compliance

### How it works

1. Subscribe to this server
2. Enter your Jitbit Help Desk URL, username, and password
3. Start managing tickets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Teams** — manage ticket queues and respond to customers
- **IT Teams** — track internal helpdesk requests and SLA compliance
- **Team Leads** — monitor agent performance and workload


## Available Tools (6)
- **create_support_ticket**: Add a new ticket
- **get_ticket_details**: Get details for a specific ticket
- **list_kb_articles**: List knowledge base articles
- **list_ticket_categories**: List helpdesk categories
- **list_tickets**: List helpdesk tickets
- **list_account_users**: List helpdesk users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jitbit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all open tickets and the ones approaching SLA breach."

**🤖 AI Agent:**
> Open tickets: 23. By priority: Critical (2), High (5), Medium (10), Low (6). SLA at risk (< 2 hours remaining): 1) #4521 — 'Login page 500 error' (Critical, 45 min left). 2) #4518 — 'Payment processing failed' (High, 1h 20m left). Breached: 1 ticket (#4515, 'Email sync issue', 3h overdue). Would you like to respond to the critical tickets?

---

**👤 You:**
> "Create a new ticket for server maintenance and list all categories."

**🤖 AI Agent:**
> Ticket created! #4524 — 'Scheduled Server Maintenance — DB Cluster'. Category: Infrastructure. Priority: Medium. Assigned to: DevOps Team. Categories: 8 total. Infrastructure (12 tickets), Account Issues (8), Billing (5), Feature Requests (15), Bug Reports (23), General (4), Onboarding (3), Security (2).

---

**👤 You:**
> "Reply to the critical login error ticket and update its status to In Progress."

**🤖 AI Agent:**
> Reply sent to #4521! ✅ Content: 'We've identified the root cause — a misconfigured load balancer rule. Our DevOps team is applying the fix now. ETA: 30 minutes.' Status updated: New → In Progress. SLA timer paused. Assigned to: Mike Torres (DevOps). Would you like to add an internal note or check other tickets?


## ❓ FAQ

**Q: Can I manage tickets and reply to customers through the AI agent?**
Yes. List tickets with filters, inspect individual tickets with full history, create new tickets, update status, and reply to customers or add internal notes.

**Q: Does Jitbit require a self-hosted URL?**
Yes. Jitbit can be self-hosted or cloud-hosted. Provide your instance URL (e.g., `https://helpdesk.company.com`), username, and password. Authentication uses HTTP Basic Auth (Base64 encoded) against `{url}/api`.

**Q: Can I track SLA compliance across tickets?**
Yes. Tickets include response and resolution time metadata. Monitor SLA compliance by checking time-to-first-response and time-to-resolution against your SLA targets.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jitbit](https://vinkius.com/mcp/jitbit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jitbit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jitbit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jitbit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jitbit": {
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
