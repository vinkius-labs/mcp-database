# Mailingwork MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailingwork)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Execute professional email marketing campaigns with advanced segmentation, A/B testing, and GDPR-compliant list management.

## Description
Connect your **Mailingwork** account to any AI agent and manage email campaigns through natural conversation.

### What you can do

- **Campaign Management** — Create, schedule, and track email campaigns
- **Subscriber Lists** — Manage mailing lists with import and segmentation
- **Report Analytics** — Access open rates, click maps, and delivery metrics
- **Deliverability** — Monitor bounce rates and sender reputation
- **Template Management** — Browse and manage email templates

### How it works

1. Subscribe to this server
2. Enter your Mailingwork username and password
3. Start managing campaigns from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Email Marketers** — run campaigns with detailed analytics
- **German Businesses** — GDPR-compliant email marketing
- **Agencies** — manage multi-client email programs


## Available Tools (10)
- **create_subscriber**: Create a new subscriber
- **get_mailing**: Get mailing details
- **get_subscriber**: Get subscriber details
- **list_lists**: List all subscriber lists
- **list_mailings**: List all mailings/campaigns
- **list_subscribers**: List all subscribers
- **list_tags**: List all tags
- **send_transactional_email**: g., order confirmation).

Send a transactional email
- **trigger_automation**: Trigger an automated workflow
- **update_subscriber**: Update an existing subscriber


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mailingwork** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all campaigns and performance for this month."

**🤖 AI Agent:**
> Campaigns (April): 6 sent. 'Spring Newsletter' (3,200 recipients, 38% open, 8% click ⭐). 'Product Update' (2,800, 32% open, 6%). 'Webinar Invite' (1,500, 45% open ⭐, 12% click). 3 others. Total sent: 12,400. Avg open: 35%. Avg click: 7.2%. Bounces: 1.1%. Unsubscribes: 0.3%.

---

**👤 You:**
> "Show mailing lists and subscriber growth."

**🤖 AI Agent:**
> Lists: 4. 'Main Newsletter' (3,200 subscribers). 'Product Updates' (2,800). 'Webinar Attendees' (890). 'Partner Newsletter' (450). Total: 7,340. Growth (30 days): +180 new, -25 unsubscribes. GDPR consent: 100% confirmed. Double opt-in: enabled.

---

**👤 You:**
> "Show click map and deliverability report for the Spring Newsletter."

**🤖 AI Agent:**
> Spring Newsletter click map: 'Shop Now' button (142 clicks, 55%). 'Read More' link (68, 26%). 'Social links' (34, 13%). 'Unsubscribe' (15, 6%). Deliverability: Delivered: 3,168 (99%). Soft bounce: 22 (0.7%). Hard bounce: 10 (0.3%). Spam: 2 (0.06%). Inbox placement: 96% (estimated).


## ❓ FAQ

**Q: Can I manage campaigns and track delivery?**
Yes. Create and schedule campaigns, track opens, clicks, bounces, and monitor sender reputation.

**Q: Does Mailingwork use Basic Auth?**
Yes. Mailingwork uses **HTTP Basic Auth** with username and password against `api.mailingwork.de/webservice/v2`.

**Q: Is Mailingwork GDPR-compliant?**
Yes. Mailingwork is a German email platform built for GDPR compliance with data processing in EU data centers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailingwork](https://vinkius.com/mcp/mailingwork)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mailingwork** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mailingwork` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mailingwork** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mailingwork": {
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
