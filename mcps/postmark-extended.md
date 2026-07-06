# Postmark MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/postmark-extended)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate transactional email delivery via Postmark — manage servers, templates, and bounces directly from any AI agent.

## Description
Connect your **Postmark** account to any AI agent and simplify your transactional email management, deliverability tracking, and template orchestration through natural conversation.

### What you can do

- **Email Delivery** — Send single or bulk transactional emails programmatically directly from your agent using verified signatures
- **Template Management** — Query and manage your catalog of email templates to ensure consistent messaging across your server
- **Bounce Tracking** — Access a history of bounced emails and monitor deliverability issues in real-time
- **Server & Account Control** — List and manage your Postmark servers and account settings programmatically
- **Engagement Insights** — Access aggregate performance analytics, including sent and open metrics

### How it works

1. Subscribe to this server
2. Enter your Postmark Server Token (and optional Account Token) from your settings
3. Start managing your transactional emails from Claude, Cursor, or any MCP-compatible client


## Available Tools (11)
- **list_outbound_messages**: List sent messages
- **list_account_servers**: List account servers
- **list_email_templates**: List email templates
- **send_batch_email**: Send emails in batch
- **send_email**: Send a single email
- **get_server_info**: Get Postmark server configuration
- **get_delivery_stats**: Get email delivery statistics
- **get_outbound_stats**: Get outbound delivery stats
- **get_template**: Get details for a specific email template
- **list_bounces**: List recent email bounces
- **list_domains**: List all verified sending domains


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Postmark** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a transactional email from support@example.com to john@doe.com with subject 'Reset Password'."

**🤖 AI Agent:**
> I've sent the email. The message ID is '123-abc-456' and it was successfully accepted by Postmark.

---

**👤 You:**
> "Show me all email bounces from the last 7 days and identify the main failure patterns."

**🤖 AI Agent:**
> 47 bounces in the last 7 days (1.2% bounce rate). Hard bounces: 28 (invalid addresses), Soft bounces: 14 (mailbox full), Spam complaints: 5. Top offending domain: outlook.com with 12 bounces. 8 addresses were auto-suppressed after repeated failures. Your sender reputation score remains healthy at 97/100. Recommendation: clean 28 invalid addresses from your mailing list to maintain deliverability.

---

**👤 You:**
> "Send a transactional welcome email to new user sarah@meridian.io using the onboarding template."

**🤖 AI Agent:**
> Welcome email sent successfully via Postmark. Recipient: sarah@meridian.io. Template: "Onboarding Welcome v3" (ID: tpl_2847). Subject: "Welcome to the platform, Sarah!". Message ID: msg_9f3a2b. Delivery confirmed in 0.8 seconds. The template automatically personalized the greeting, included the quickstart guide link, and set the first follow-up email to trigger in 24 hours.


## ❓ FAQ

**Q: Can I send a transactional email using my AI agent?**
Yes! Use the `send_email` action. Provide the sender and recipient details along with your subject and message body.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/postmark-extended](https://vinkius.com/mcp/postmark-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Postmark** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `postmark-extended` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Postmark** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "postmark-extended": {
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
