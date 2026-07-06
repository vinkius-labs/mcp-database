# Mailgun (Transactional Email & Domains) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailgun-transactional-email-domains)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage email infrastructure via Mailgun — send transactional emails, monitor domain health, and audit delivery logs.

## Description
Connect your **Mailgun** account to any AI agent and take full control of your transactional email delivery, domain health, and suppression management through natural conversation.

### What you can do

- **Transactional Messaging** — Send high-priority transactional or marketing emails directly from your agent, specifying verified domains and custom text bodies securely
- **Domain Health Audit** — Retrieve detailed DNS records and state mappings for your domains, including SPF, DKIM, and MX dependencies to ensure deliverability
- **Suppression Management** — List and audit bounced emails, unsubscribes, and complaints, with the ability to selectively delete suppressions to allow resending
- **Analytics & Statistics** — Query domain-level analytics to track open rates, click-through rates, and general delivery performance in real-time
- **Event Logging** — Extract raw chronological event logs (deliveries, opens, drops, bounces) to investigate delivery failures or anomalous traffic spikes
- **Email Validation** — Use the Mailgun Validation API to check if an email address is deliverable and valid before initiating a send request
- **Template Discovery** — List and retrieve stored HTML Handlebars templates associated with your domains for consistent professional messaging

### How it works

1. Subscribe to this server
2. Enter your Mailgun Private API Key
3. Start managing your email infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Developers** — test transactional email flows and validate domain settings through natural conversation without manual API tools
- **DevOps & SREs** — monitor domain deliverability and investigate delivery logs directly from your workspace for rapid incident response
- **Growth Engineers** — audit campaign stats and manage suppression lists across multiple Mailgun domains efficiently


## Available Tools (10)
- **get_stats**: Get analytics and stats for a Mailgun domain
- **get_templates**: List email HTML templates for a Mailgun domain
- **list_domains**: List all configured domains on the Mailgun account
- **list_logs**: List raw event logs (deliveries, opens, drop, bounces) for a domain
- **list_unsubscribes**: List unsubscribed emails for a Mailgun domain
- **send_email**: Send an email using Mailgun
- **validate_email**: Validate an email address via the Mailgun Email Validation API
- **list_bounces**: Useful to detect out of bounds sending or inactive audiences.

Check bounced email logs and suppression list for a domain
- **delete_bounce**: Irreversible action.

Delete a bounced email from the suppression list
- **get_domain**: Get domain details and DNS records for a Mailgun domain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mailgun (Transactional Email & Domains)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a transactional email to 'user@example.com' from 'support@mg.domain.com' with subject 'Order Confirmed'"

**🤖 AI Agent:**
> Dispatching email… I've successfully sent the message to 'user@example.com' via the 'mg.domain.com' domain. The Message ID is '202603271234.abc@mg.domain.com'. Would you like me to monitor the event logs for delivery status?

---

**👤 You:**
> "Check the DNS health for domain 'mg.mycompany.com'"

**🤖 AI Agent:**
> Retrieving domain details… For 'mg.mycompany.com', SPF and DKIM records are verified and active. However, the MX records are currently marked as 'Unverified'. You may need to update your DNS settings to receive replies. Would you like the exact MX values to add?

---

**👤 You:**
> "List all bounced emails for 'mg.mycompany.com' from the last hour"

**🤖 AI Agent:**
> Retrieving bounce logs… I've identified 3 bounced addresses: 'old-user@gmail.com' (5.1.1 User unknown), 'invalid-addr@yahoo.com', and 'full-mailbox@outlook.com'. Would you like me to remove 'full-mailbox@outlook.com' from the suppression list so you can try again?


## ❓ FAQ

**Q: Can I check if my domain's DNS records are correctly configured?**
Yes. Use the `get_domain` tool by providing your verified domain name. Your agent will retrieve the status of SPF, DKIM, and MX records, helping you identify if any DNS dependencies are missing or misconfigured.

**Q: How do I see which emails have recently bounced from my domain?**
The `list_bounces` tool allows your agent to extract the suppression logs for a specific domain. You'll see the email addresses that failed to deliver, providing insights into audience health or sending boundaries.

**Q: Can my agent validate an email address before I send a message?**
Absolutely. Use the `validate_email` tool to check if an address is valid, deliverable, and doesn't belong to a disposable service. This is perfect for ensuring high-quality data before triggering outbound sends.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailgun-transactional-email-domains](https://vinkius.com/mcp/mailgun-transactional-email-domains)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mailgun (Transactional Email & Domains)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mailgun-transactional-email-domains` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mailgun (Transactional Email & Domains)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mailgun-transactional-email-domains": {
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
