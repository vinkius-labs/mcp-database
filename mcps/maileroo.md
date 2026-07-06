# Maileroo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/maileroo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Deliver transactional emails reliably at scale with an SMTP relay and API that prioritizes inbox placement and speed.

## Description
Connect your **Maileroo** account to any AI agent and manage transactional email through natural conversation.

### What you can do

- **Email Sending** — Send transactional emails with templates
- **Address Verification** — Validate email addresses before sending
- **Delivery Tracking** — Monitor delivery status and inbox placement
- **Bounce Management** — Track bounces, complaints, and suppressions

### How it works

1. Subscribe to this server
2. Enter your Maileroo API Key
3. Start sending email from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — integrate transactional email into workflows
- **Operations** — monitor delivery rates and bounces
- **Product Teams** — manage email templates and verification


## Available Tools (6)
- **list_sending_domains**: List sending domains
- **list_email_templates**: List email templates
- **list_configured_webhooks**: List webhooks
- **send_transactional_email**: Send a transactional email
- **get_domain_details**: Get details for a specific domain
- **list_sending_activity**: List recent sending activity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Maileroo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify an email address and send a welcome email."

**🤖 AI Agent:**
> Verified! ✅ sarah@company.com — Valid, deliverable, no disposable domain. MX records: OK. Email sent! To: sarah@company.com. Subject: 'Welcome to our platform'. Template: 'welcome_v2'. Status: Delivered ✅ (1.2s). Message ID: msg_4521.

---

**👤 You:**
> "Show delivery analytics and bounce report."

**🤖 AI Agent:**
> Delivery (7 days): 1,245 sent. Delivered: 1,208 (97% ✅). Bounced: 28 (2.2%). Soft: 18, Hard: 10. Complaints: 3 (0.2%). Avg delivery time: 1.8s. Suppression list: 45 addresses. Top bounce domain: outlook.com (8).

---

**👤 You:**
> "Bulk verify a list of 5 email addresses."

**🤖 AI Agent:**
> Bulk verification complete! 5 addresses. ✅ Valid: 3 (sarah@company.com, mike@techco.io, lisa@startup.com). ⚠️ Risky: 1 (info@temp-mail.org — disposable domain). ❌ Invalid: 1 (john@nonexistent.xyz — MX not found). Recommendation: Remove 1 invalid, flag 1 risky.


## ❓ FAQ

**Q: Can I send transactional emails and verify addresses?**
Yes. Send emails with templates and verify addresses for deliverability before sending.

**Q: How does Maileroo authentication work?**
Maileroo uses a custom **X-API-Key** header against `api.maileroo.com/v1`.

**Q: Can I track bounces and delivery rates?**
Yes. Monitor bounce rates, complaints, suppressions, and overall delivery metrics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/maileroo](https://vinkius.com/mcp/maileroo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Maileroo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `maileroo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Maileroo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "maileroo": {
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
