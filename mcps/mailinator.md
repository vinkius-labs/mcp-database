# Mailinator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailinator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Test email workflows with disposable inboxes that catch every message without touching production mailboxes or real addresses.

## Description
Connect your **Mailinator** account to any AI agent and manage email testing through natural conversation.

### What you can do

- **Inbox Browsing** — Browse public and private inboxes with message lists
- **Message Reading** — Read email content, headers, and attachments
- **Domain Management** — Manage private domains and routing rules
- **SMS Testing** — Access SMS messages and phone number inboxes
- **Webhook Testing** — Monitor incoming webhooks and payloads
- **Rule Management** — Configure inbox rules and forwarding

### How it works

1. Subscribe to this server
2. Enter your Mailinator API Token
3. Start testing email from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Engineers** — test email flows and notifications
- **Developers** — debug email delivery in staging environments
- **DevOps** — monitor email infrastructure and routing


## Available Tools
- **remove_message**: Delete an email
- **list_message_attachments**: Get email attachments
- **get_domain_details**: Get domain metadata
- **extract_message_links**: Get links from email
- **get_message_content**: Read email content
- **get_usage_statistics**: Check API usage
- **inject_test_message**: Simulate incoming email
- **list_private_domains**: List your domains
- **list_inbox_messages**: List messages in inbox
- **list_routing_rules**: g. forward, click-all).

Get inbox rules
- **list_private_sms**: Check SMS inbox
- **list_active_webhooks**: Get notification configs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mailinator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the inbox for test@privateteam.testinator.com and read the latest message."

**🤖 AI Agent:**
> Inbox: test@privateteam.testinator.com. Messages: 5. Latest: Subject: 'Password Reset Confirmation'. From: noreply@app.com. Received: 2 min ago. Body: 'Hi Test, click the link below to reset your password: https://app.com/reset?token=abc123. This link expires in 30 minutes.' Headers: SPF ✅, DKIM ✅, Content-Type: text/html.

---

**👤 You:**
> "Show all private domains and their inbox counts."

**🤖 AI Agent:**
> Private domains: 3. 'privateteam.testinator.com' (12 inboxes, 45 messages). 'staging.myapp.io' (8 inboxes, 23 messages). 'qa.testing.dev' (5 inboxes, 18 messages). Total: 25 inboxes, 86 messages. Rules: 4 active forwarding rules. Oldest message: 7 days (auto-purge: 24h for free, 30d for team).

---

**👤 You:**
> "Check SMS inbox and show webhook test results."

**🤖 AI Agent:**
> SMS inbox: +1-555-0123. Messages: 3. Latest: 'Your verification code is 847293' (from: MYAPP, 5 min ago). '2FA code: 123456' (from: AUTHSVC, 1h ago). Webhooks received (24h): 8 total. POST /webhook/stripe (3, all 200 ✅). POST /webhook/twilio (5, 4x 200, 1x 500 ❌ payload error).


## ❓ FAQ

**Q: Can I browse inboxes and read emails?**
Yes. Browse public and private inboxes, read full email content including HTML, headers, and attachments.

**Q: How does Mailinator authentication work?**
Mailinator uses a custom **Token** header for authentication against `api.mailinator.com/api/v2`.

**Q: Can I test SMS messages too?**
Yes. Access SMS inboxes and read SMS messages for phone number-based testing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailinator](https://vinkius.com/mcp/mailinator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mailinator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mailinator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mailinator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mailinator": {
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
