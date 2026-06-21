# SendGrid MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sendgrid)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Deliver transactional and marketing emails at massive scale with industry-leading deliverability and real-time analytics.

## Description
Connect your **SendGrid** account to any AI agent and take full control of your email delivery and marketing orchestration through natural conversation. SendGrid provides a world-class email infrastructure, and this integration allows you to send transactional messages, manage recipient lists, and monitor delivery statistics directly from your chat interface.

### What you can do

- **Transactional Email Orchestration** — Send instant or scheduled emails using dynamic templates or custom HTML programmatically.
- **Marketing Contact Management** — Access and monitor your contact database and create recipient lists for your campaigns directly from the AI interface.
- **Engagement & Stats Intelligence** — Retrieve real-time email statistics, including delivery rates, opens, and click-through data via natural language.
- **Sender Identity Control** — Manage verified sender identities and monitor global suppressions to ensure your domain reputation is always protected.
- **Operational Monitoring** — Track spam reports and retrieve account profile metadata using simple AI commands to ensure your email operations are optimized.

### How it works

1. Subscribe to this server
2. Enter your SendGrid API Key from your dashboard settings
3. Start managing your email infrastructure from Claude, Cursor, or any MCP-compatible client

No more manual stat exporting or complex SMTP configurations. Your AI acts as a dedicated email operations manager or delivery coordinator.

### Who is this for?

- **Developers & DevOps** — quickly send test emails and monitor delivery logs without switching tools.
- **Marketing Engineers** — automate the management of marketing lists and track engagement metrics via natural conversation.
- **Operations Teams** — streamline the retrieval of account statistics and monitor verified sender health directly within the chat.


## Available Tools
- **create_marketing_list**: Create a new marketing list
- **get_account_info**: Get SendGrid account details
- **get_email_stats**: Get account-wide email statistics
- **get_template**: Get template details
- **list_marketing_contacts**: List marketing contacts
- **list_ip_access**: List allowed IP addresses
- **list_marketing_lists**: List marketing segments/lists
- **list_spam_reports**: List spam reports
- **list_templates**: List dynamic email templates
- **list_verified_senders**: List verified sender identities
- **send_email**: Use JSON strings for recipients and dynamic_template_data.

Send a transactional email
- **upsert_contacts**: Use JSON array of objects.

Add or update marketing contacts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SendGrid** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a welcome email to test@example.com using template 'd-12345'."

**🤖 AI Agent:**
> Processing email delivery... Your welcome message has been successfully accepted by SendGrid for delivery to test@example.com.

---

**👤 You:**
> "Show me the email deliverability metrics and domain reputation for all verified sender domains."

**🤖 AI Agent:**
> 3 verified sender domains. "yourcompany.com": Reputation score 95/100 (Excellent). DKIM: valid, SPF: valid, DMARC: enforced. Deliverability: 98.4%. Bounce rate: 0.8%. Spam rate: 0.05%. "marketing.yourcompany.com": Score 89/100 (Good). Deliverability: 97.1%. "transactional.yourcompany.com": Score 97/100. Deliverability: 99.2%. Total emails sent today: 12,340. Global suppression list: 234 addresses. IP warmup status: fully warmed (all 4 IPs).

---

**👤 You:**
> "Send a transactional email using the order confirmation template to a customer."

**🤖 AI Agent:**
> Email sent via SendGrid. To: customer@email.com. Template: "Order Confirmation" (d-a1b2c3d4). Dynamic data populated: order number #ORD-2025-456, 3 items totaling $189.97, shipping address, estimated delivery May 22. From: orders@yourcompany.com. Message ID: msg_abc123. Delivered in 0.6 seconds. Open tracking: enabled. Click tracking: enabled on CTA buttons. Categories tagged: "transactional", "order-confirmation". Webhook events will fire for open/click/delivery.


## ❓ FAQ

**Q: Can my AI automatically send an email using a SendGrid dynamic template?**
Yes! Use the `send_email` tool. Provide the destination email and the Template ID, and your agent will deliver the message via SendGrid's infrastructure instantly.

**Q: How do I check the global email statistics for my account?**
Simply ask the agent to run the `get_email_stats` action. Provide a start date, and it will retrieve aggregate metrics including requests, delivered, opens, and clicks.

**Q: How do I find my SendGrid API Key?**
Log in to your SendGrid dashboard, navigate to **Settings** > **API Keys**, and click 'Create API Key' to generate your unique secret key (SG.xxx).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sendgrid](https://vinkius.com/mcp/sendgrid)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SendGrid** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sendgrid` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SendGrid** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sendgrid": {
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
